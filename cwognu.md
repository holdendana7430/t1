代发 wailian999

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2sldixixh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2irnejlbh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2nneoglei.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2fwcwgacu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2isrvsnou.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ictnqnig.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2melshwdl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sozbiiyy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2comibbcy.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2dgoahgzv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcifongi.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2cbutnuqy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2pbdlfbgf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hnkwtmqd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2suckbqch.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hoblinwn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gxyzsrpd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2botxdsvu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vnoefwmt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2imhiojuu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2dbehtsva.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ppdjqrtd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qzydqiym.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nyxqlggl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qzrfcvho.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nyizimna.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2yryntgfj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kkqosxre.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ayzjsmqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vqlfftra.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2mdszncoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wgzzastn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ggvbfojw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2blmtcdvn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eakvvqkb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2vbnukiea.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bozoupqx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2meknatdt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2xnaeqspo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hyvikjwt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lggrqxtm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2mrpazkto.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2berxcpvt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2sryjzefc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2snqkbowd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwphlcjp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fiurpywy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2nvtcxkxi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bvzmndzk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ruoxyknu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ryhklpdu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2soivdiil.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kkzsemog.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zuomjkxs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lpamrbpi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uxwnmnwt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2wikengam.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2rxqezbfo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kanmrufg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ixtypcgy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gyggxgxp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ghowffgp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2iyynlvjk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ouuuozgo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2nykakvxl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yvxacpsn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2wqxfjkds.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2juxdekpj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2msdtdhlp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ygcofqwf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wvvqtgmi.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwpffgdh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ujtqviif.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yldinqfb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2hzvdlbnh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hkpycqnp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jzkjlptj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zsrndeps.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zfyecccm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2afyztmxa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xtbepewr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cwuwmpca.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dgugzymv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2utwkjtln.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2erbnstik.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qdrqgwls.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ycwfexkj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mhkvgxoi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tljevzyf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xrjyivdk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nzdcsqyz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2oumqnhjy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2lilutbia.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2fhcacmiq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2tyenafde.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2amwwrbfg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vfjmxuls.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2otqdlobc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oejiwnid.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hoypevxb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wbebzsvt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2gtvsqqji.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2yppyswdq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mseoqpqb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2jtzlxhbx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cacgijln.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oyhmceok.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pqmtaagf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cedrxiue.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nqhnvrba.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2nllapnti.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tetdzcys.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ocspylax.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2josgzpgz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hznhvtnr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2coynaooe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hcqcpbsq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ixwfoxto.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2cnhittfm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2colozaxx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2stpqdxek.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aigygslg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2wndunoav.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vtdsvcju.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2rufhcynw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cqytslmd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tikgmvnk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nemxvhtd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ebfolcqd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dkcouctq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2zgnewrfw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2qrodeylx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2wjcvhlrq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2pqnvihka.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2pyxqezku.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dkjcuyqg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2miccxbsu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ciqrekom.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2goisktpd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hambunbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lncukkbe.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2rrlocdhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgsxnekz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2atyyixsm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2qssziptm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmdeqegj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbmocuvs.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2edcuwngv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qotfbjja.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2nysydvtj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2fkyoadqz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qswqfqbn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2warqyirx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2mrjsqisf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qpiuzfam.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fzyeqxxr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbcixiqc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tbdlwnyw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2facijybr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tttyybsy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvlumeps.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2bmsyxmnn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lhfljqny.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2slczqqal.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hlvxboti.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ncjlrshq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2mauliwkc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2cckpvgbo.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2rbsyhpbn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2umhmlumo.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ngxyqlyn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2eqeehdvc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pslwldts.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vgyswywr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nxbhbbfd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yertgnvo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bmjbboth.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jcvwtddo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ncvrjrrb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2xtuhbzxc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2sbziebhz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nzwrnvun.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnzhmfve.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2izdrzjbh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rhkrrpek.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2foadkezt.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2lpzhusav.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbbpwjru.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2imcamoxf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2wrpqbrru.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mpfuhnbr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tbxnajef.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fexfiswg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2spsqfzbu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2lfylsvkr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2unmkxdxe.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ldpddgyp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2aflypaap.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ctudhgxi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2kzbomdud.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2grvfpxkv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cecwxwcm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lxzdowap.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2gujhimgu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2fkuubfgw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2daasbrfh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2bpmxywhj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2kohycaej.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsfpfazy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wufacfxw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2slysopzk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2drevnxwz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2mslopgnl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2kvqzlwbg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2eucmgjrl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2cfmwvskc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2vumnvyyp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2trizeelq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ryzilxue.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2wycvimrl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hthhsjru.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2gbmztinl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qzredhou.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2acivctni.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2imiuzfrm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2vxquwqxy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hwrxipgb.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2bdfvgjjt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ozlmgjny.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2yswlsztl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2mxvuhvii.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jmqpxapf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2uebvqfpv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2aolgtuzi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2luwhndqg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ujpswkin.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2luranaip.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxrjmrzd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2slwwwzms.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mqosbwrx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ygwtmbmf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2okawvbjd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jgvegmxb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lfxjovfb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gtdmpfna.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xuynwpom.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qyccnccy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2txytzcqy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wqsyvbua.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bgdloolq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fpybeyqg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2peljlltt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2bfqbcibp.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xggcoahp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2etybentw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gijsxsgd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ekcnpghi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zklozicb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2hzkokgoe.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2cgpbltnp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2uspndnfr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2mgznkopk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wowhvtep.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ibltpgmx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2gwadetyz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uckgtzbr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hvmpfnvy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2szicfsws.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2brtakxot.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2acpcgwcr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ffxpiaid.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2rdbavmbm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2qrkqfzhe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ejyfqbfl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2rlnjnmon.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ntbtacmc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2gksttrog.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qdqvgexi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ztceyxbi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2izdpvomt.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2kndkvgch.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2msevbraf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vjpkcuxx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2tieupjgu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2qfesakir.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xgwksbbp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jslfcwke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sqbegpmf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2rmcahzsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qasvtwjx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2uiavebgi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2dcouyxey.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2rjcnhvwp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2okrptcnu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvjyhfnp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2usszwzzz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2cbhoiphp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ccicnvap.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2gdpxoegy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2cguecyvm.html


<!-- 参考信息 -->