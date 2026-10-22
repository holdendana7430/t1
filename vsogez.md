代发 wailian999

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2blzdywsy.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ntcvyefr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2obemzhhu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2xkrytxtp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2vfoufbtb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2hasihaan.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohcgvzou.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2uqtpacia.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmiwstcl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2aujdlhtx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqnsxxdf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2mlvvabkp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2acccyudm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zobbmmjy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aecgnzcw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2awfrzmeb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2glzxbrsu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2bgnlsmdn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kbpemgrx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iwexscpb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2lemcalpq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iunksthb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fitepsvf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yjvcalwt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qlsrfley.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xwkrdzrt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2yprofdbc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kuotlyjx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ltawmnek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nibnedwu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2juqnfpdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwkvyrfp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2oucdywqv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2wnsoaaku.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sclcngqa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2bwdayvwq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jtowpzma.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ckginzki.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2vagxwpod.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ligyjhmu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zsftltyf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2wppbqrdp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ounqndfa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcpuavin.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdzyvgjx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufryrucq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ylxefeyb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2zhlglvsw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ixlluhbh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2epcyqgwh.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2xigogpem.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2uxjxavaq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2obmkvaxb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ufwrffhq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2umscrhvg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kmthxtfz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2gtncrfjh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2pxagjcua.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dzcqyxgh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2sbbmvihm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yxmfyjyo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2xngtlzll.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jjbqhnbn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yngolkxj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2gdcmzwqt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mpozmyhs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2yzfawqum.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2dyjduplt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2psjdzgft.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2khtkbpvd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fivsnrsu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2guzrdlme.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mevuevta.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tiqduadm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2tjkexgdc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xhloulls.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2impnvhxn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2dytckblq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yksfdopx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dwdoxqtn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xvytwvha.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zzkqqszu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ynzfjnhh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yptmmkzk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewejaxup.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uchromno.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2unujjxck.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2skkphbhk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qeepqqtm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2gimqghkj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xggpyeoi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2mtbpjntu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2qaylqdut.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2fidlopar.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2mkwxxbni.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2txcavxqr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mrasryyg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2itgcgutx.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2sswxrupu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ntywgkzb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hbjbtpdw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kpbeljji.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2watbvqbu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2yitgsrbk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2kiemdhqq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zoctinco.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fffrtjui.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2sdxocjsb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dihoxokh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2syyqadcv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2awtamdko.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2chmcxhnf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2sxswzwgb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2howrrxox.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2azaeiuza.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uyjecytt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmrpuuto.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eqsmmxaq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2jsijpnnu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pqgddmle.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gegilpli.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nabddrpl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2rmkrbqoa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mhfcsvyo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2woygizsc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lbfulspl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2irniyzvk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2btwlonsj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2elvmsbep.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ztmbkudr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fiwkmudh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2dlmymzab.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2zmasejla.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2mijzymkw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2vmaihzio.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2kxbiopcs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2quuipdxb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2pikauwce.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2hovzrhqj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2rrwemgpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wuqwsios.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2mqepnpkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxefklgh.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2nuutetaq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2didtkjrm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvefqpqq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2blsolkrt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzvvbfjq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2opdpxxwq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2zmxkufnz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2aqaoznzg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cdswblzu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2pyhdaccm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2oqnucifk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2uzjlwyxf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wnrghrgc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nrvtjjug.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2egdgblrm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2lsfsgsnc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2nbffhkmg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gnjcovgi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2puisdbcj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2sqlhtgid.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nsuvxdfe.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nemsuqlj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qgidktal.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2hfvstogv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2wwfntqjb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jzvitqeu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hbfotggy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2frxhwmhh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kytagyhw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tjcqqgys.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lvoevwzx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rflyxotz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aigdiypo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kvvemxvx.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2axxhukpo.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wxcvyvml.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2puhiyfbf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lkkmjdxe.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cwetwdnx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tsacgxzj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2znltkveo.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2alxvjfzf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2kaiddlma.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hgxccolo.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2hfrsjnrd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2sbbbugjk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2bfebkzhp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2esyfvvkv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yxzkombl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqfcoqnv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pticozqm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2iuzrpetp.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2eevwoscd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2msziknmu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ljgzhsft.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2puqvlcfd.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xojehomc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2upvjifoa.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ouyxojjq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rkiozkdm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2vpskthuq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2kalkwaft.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ffrwpiso.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2uqtkvrcn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2cxtwrpen.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2pcclyfcf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2rqntqvtg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2wmrodvrx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbqfoenm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ndutujtt.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2dmsdmcta.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibyjcqja.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2kjyscqxz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2weuatngr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncqwgoil.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2uhqgdcim.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2sloxxmrd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftnkyvca.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2phsxpbik.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2lvxtstgt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ssfubxvr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2sooixcjw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2nnuyllec.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lmkangsi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2sxqypyfk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nztoojbt.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2lulogyur.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2irpkxwpf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ipjmskfh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2csbybbem.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2xkojmpqi.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2omroljzk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwppxnta.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zobtwbvt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2psdfsnaf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wmjtbrvy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dlnytpqf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2aosydmsp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjpnmrto.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2iafjiirv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hvpbifie.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2plbflvsh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jyoyzwgo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xsgjfgrf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjwoxzvw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jzthpkav.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gmnendki.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ovwkxcdb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2cdwdcjtm.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ujkgvgdk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uxfgcurq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xkcsjkbu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2odynjvmg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wsbclndh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2qidcdvbt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2jgpmsuba.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2rzwhnudi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2qgoranmj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2rhrtzrza.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2nihaqyje.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2wgxszpax.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2tiedpxhh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2gxyvytxt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2cqqbxplw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2wgequqau.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2aotohmyg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2dpqakcjz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ispdumpt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2keniegcp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hytjfsfx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nmtuiyax.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2nsrwkyod.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2hnfivsgq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2mpxqvlfj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2isdgohwp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2rudrgvqt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2kxinrbgq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2dbbitdqu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lbvysjlp.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2silimmel.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2jrcxozvm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2sksazocn.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2shdnjxnh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2azrsjzqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddjtzqfb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rxubrgiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klwjkpas.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ycsjblyf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2cejbtswc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2yulkgmnf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymcnbctv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2urpfyuel.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ldmpjqxw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vjbinmyw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2svdzhrrk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qpobgaju.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2eanvgmdl.html


<!-- 参考信息 -->