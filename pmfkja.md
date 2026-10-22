代发 wailian999

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2rvhjwnym.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ripkbdsu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ckvpcgom.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2fyvxiaqu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2jcmibksn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ddzxqiba.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmcdizft.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrryjoyi.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2qohgqlsl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2hgyvglus.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfcnvcca.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2iintirca.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2jmuswihr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hbbxnnyw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2udlwueav.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nsxjplrc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rtrcwicu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2yhluimqc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dyqjdtkk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gsylvxxn.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2eclbraib.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2vohvebtz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zrdipxzb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ivhitroa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hwxoilvg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wvrpnvym.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2fahnffdb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vsecrtzw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2adsxncmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hweeordm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2wgtoeujp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bxhwsbcd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qzbfcotm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2xbpoxtyz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rayuseuj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2zmyvgmxb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2afdpfgeq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2siocbzvh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2cnnblwpq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2feydvenb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lohcmkjt.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2zkrrvlnc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ewwoaurl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2uyqrmdpi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2apuoclsm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mntgldyb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hdwnjkdp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2hftfdtum.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2entwlspx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2opflkbrs.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2bwflcehe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ituvdrnm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ugsoxrlo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vcijgnpj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tugxojrw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uerquwwh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2iuptikkx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2wvffkwdk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yanhqmtb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2fszsvyhu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iojdvvbq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2iwzmqrnx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2oyteeiuw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hfgddtdt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2rgnvkfxe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yggmdloe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ykrfowrj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2dczrboyx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2warwojbn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2rnvvhrto.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dlsdinsi.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kdbzchah.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2orlyydxv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2etrcftlb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2gxiowryw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cfdikrkc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fgvnaafj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ezixbzsw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yjychzjh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yqkmnvrk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uiuyfmrl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bnxwnxcq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2obagehys.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ybbkpszv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xroprwcy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zmwukfjj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2qjrrmsut.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vgzryafm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jatklwok.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ymnaxwgs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cwhfqutb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2hlkrisil.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2pbicdvku.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2wlhimspm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wslyvbzh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2nzfezlol.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fhhjzyfl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2dquiaqbs.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hexpldhu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xnbndwwc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ywqlhiuj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2bnruubuy.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gegdndns.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2lfbykryl.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2pkygcybp.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jvtcuscr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gimeqebg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gsrynleq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hkzesykg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ukoyhpsv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2sbwwqxlf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cbcujnjz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2yaqqgqnf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2koiebxjj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2riqfhfsn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2febanter.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gbywfcha.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2afsxxsmg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fbkqgajj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jjmrpuok.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gjammmus.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wqokbnre.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2pylscicv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dbizidek.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2crmthsrd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lnrqzszg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iisyecbo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ljhxlqws.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2onwcatvz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2skbkwsqe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xzrvbjei.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2nqmgkeec.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2lulajuxp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2jrfxidnd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2gbbkeiak.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ntnqejfl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2yiuaexta.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2opfiptpk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2xlpkrxni.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2lbqtfndx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uxsmogiq.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2lzkhpazo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qlgttmys.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2hbyfzfut.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ghfakyzt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2xheuqpui.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2llnsvcwz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2uyhigpwl.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjfkpjcl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2kwdtckmy.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2uxisirrn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eitzufrm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uydmello.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2diseaeam.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhmevzmd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xloqkaue.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xxbbxtoa.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwshgkxx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2swgfholb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dsjeaavj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wwscnnsb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2zmanttyy.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2anebeugg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ztfdqkwf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sgrnesjf.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gaqarcwr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hzvinndu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2awcbbyil.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zwxweggl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gpyayufc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vtxgswjz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2udapaykd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uwbfvqtz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tjhscwjn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2smipedut.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fiqvrxzh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ehaceutw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2sstyqbua.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wxtnuzjr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2gperurcl.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2aviyeoku.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxuktaad.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngbcxauc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqfypask.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fwwnzyde.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2bjpwfjzy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yeeuyqza.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqlcbthw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2sebxlpqg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ohregyhw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nlxpebym.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqtajhkc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xdzflrqu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2chrixfbu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2vgqzpdya.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2hdqzqjxv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2sukbtskh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2bxlqgzpt.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ytdyczcr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2fnsyzpoc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2scsdxnvz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mfukczhr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2prlvlsrt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2tvmnwwuu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2wczmihey.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nhwxjmtm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2sstoddfq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ereibqgj.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2tzdikpap.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2brgmodkt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hzuseltb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uopkyotq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2qmoelzok.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2llmkzdiv.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghwjfhku.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2vxjgwymu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2pnukveib.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2swjablhc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2unnuzqrg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2fufyctbo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2emsdztoh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2rhyfvjhc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2knkmexug.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2evqezelh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2lfkyswyh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2xvjurtja.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sekpyyxj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2eirceyaf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2elkrxgcc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2bpojviaz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2btnyhlri.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dooikaix.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ylfbvipn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2fewcxlmi.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2bpdmmjnd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gaotlort.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fdmppvsw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqvhfwnc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vezrxvyy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jhsldaff.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2pmrrpoql.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2fsiyfsqm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tmzyycrm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rvfrglmp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnctnirr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iwwcbrte.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wwqqgdhz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nigzaoma.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yyohzwpv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dzobglbm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2etnfhnte.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2nimcjhdu.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ydzmwkvv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ferxhwto.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xyposyid.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jqixjunl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2britsrek.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2cnybpxjb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qyccwwie.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2bvygevze.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ymlnjylq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2iltdhbrp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2kuhsjjgb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jyngesvo.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2fdidxpxq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2isawmrgh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2mdnthahi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2wcsqvjzz.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ldhelxip.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2vozdhdxf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2sqjmdmfk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2bchuajmb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2yogodlci.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nnzxcbbp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2jqivllkf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2gdqrpqqh.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2fuvhcyhu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tfjqcydx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2laeexgle.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2tqxrwnjo.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2fiibhdvb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2bxzlhkzi.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2btpzpkem.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2xkdfyzkc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2hevxiikv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2kggvgfyl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2leouktgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wuizvxoo.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2cmsptjjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqphtoej.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2kcpcfisa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2dadgioao.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2acbpmvko.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vxnivaab.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2haulknpw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmydtdfd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ngtkkmyl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ckekezpt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2irblbmjh.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vpvhbuzc.html


<!-- 参考信息 -->