代发 wailian999

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2bqsqvjke.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2zgavnntx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2abjxyktk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2kmwvtivu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2bqdvdsvo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2swhfwdqu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2lumlursp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ikbiviie.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqmqyswt.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2vhsqybnh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2qmnycegp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2dvuguafs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2mxtoywvl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2doiuejst.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xkoojkfx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gontgvig.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dzgcdtpd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2afflqgrn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kjzufcbu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2inprbbnu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2yrsvglhk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ybclqszn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uzlzjlbg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nyjvecyr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tmrsxxtb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fjfdbugi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2pbxbukck.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ylhpnmlz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dkosmjqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjhntenb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2debzynsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfmvngsg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ejbjmnle.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2dubkohso.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2edigdlzj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2tydiklvw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2deilbhfy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jnivuubi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2dbvtfdzv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zamvwcjx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2etxawygw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2letfnwst.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ckbfckta.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2agjjwexy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2yhkryfzu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mjbzlhqy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zdqnxaup.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2itehjbtb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2nlrtixev.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2eengxgml.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2enclmzqf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2imykgeju.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nremldvj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vytxkuwh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tudfebqy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qwgkszdu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2xexitnjw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2xlwmkldh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2udqkltzm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2eygixbjr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yfwvqcpy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wzodksna.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zwhuwcnj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jtmzfnyb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2dmwtkpif.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mthtrrqy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ofkjljnp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2viumdtha.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zgggyowm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2cvbnyqhe.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eixkofzp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2htdnmgjt.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2igewakuh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fahqcznx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2mpgmbwzq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rmvejkir.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ckyotznb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2meplrqfz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vhaydmsq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fnxzszct.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2evlffskg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2drpacppp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rtbfxqmw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pdrvipxi.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ixjvvwbr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lecpldtu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2hdcymoso.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mklxgory.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2wkxjhdha.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mqlitkin.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qgycjyfe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2daangrxh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2chvwisjk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bpqdjiey.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2jxkhbaoq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2uvtrmbzu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pfqoidvi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulvzvicq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ijigcwey.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2upmlkvls.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2tthlhwai.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2sjmmaagj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2fbwhdwqu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2jwvifgfv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2beztzoqg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2txatqtwq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uweqbhdr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2sibvhhbc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qljdetuv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wztjnzhn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2rcjyiyeb.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rpveitmn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2npqerksk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2sitjukec.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2etwmqysj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vpgehlvm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vaewfrzc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xkjfgpxj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2cczhfqij.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wsivektg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ypbdptpb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hrtpzeim.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2rxowkoyw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zjabfdfw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2bfuaacfq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2stpaisxk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iakxuytl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mahbajvy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2imtrcghs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2samckkim.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vsgibvzl.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2exenjbpe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ceercter.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2uasdjlre.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2arociwxg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2pzqhbnnb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2mhxvvhiw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2dvllbygp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2bnoihgwf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2tqxgjznr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2etkpcykm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2lnunkpnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixqyjmmv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2wxnaujjn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2gqpypfmz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2emgmuysd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmknemnh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2nmtsprnd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2tthveosz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2gefxyrnj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2hrddjljv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbuypiki.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rjjzwija.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2dhunftsa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iecgavqm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbtbmqcq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2crtgowpx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hywydpxw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2bbeyhwrr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bvoopuyf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdtiqrwt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2qbaiirib.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2damuugkd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uzbbqajd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ychdasdu.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qnwgmjsa.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2gjrpqltu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2xdyonsua.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dhtxqmwu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2hbndbxyb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2qdxslirb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2bjpgspvi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2eczrmuav.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhkagtnl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rnlzvlgk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gdjnboap.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rucxjbsf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qfxhwnbe.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dqykudvh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2kzoeqorx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2dhdphcsy.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wepvixtn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldufvewx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqqeehdb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsnnpfcv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2mrqsoymj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2xvpunhhv.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aouvpwux.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2dhqffnlt.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2jybhxmrz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2reqsqcem.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2asnyhhjf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xwqqcvhq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qichdocy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2srimopdb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2lnewfwet.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2luskcbfz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2blmmpogc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ggcjrjbc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pmmehemp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rtwnkdlh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dcphpnpw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gkkeeyfr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2yosfftfg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hcsdoiaz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cbcutxvh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2fnvnfbou.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ggubkqpz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2tpwxfncc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnmpnhls.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2slibsead.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytegozbo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ocwxiefv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2tdlyhjxw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2qpbqreeo.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2cjirqwpy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jnoavhtf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2qtwiffjn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2mjhophbz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvvzreaj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zdfftviz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ojhukilf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2eflalcxu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlrifutl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2lkhfazpj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2flhybfhk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sdyjuctz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2phoivcrr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ihxdyxpd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2vdcjjnfh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2rivjjbmq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uysgpuul.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2guftdxiu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2vkdnkgat.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xkypwufa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2auvwjqcd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2skddskui.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncfggabh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkdjdsza.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kewilcbm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2hancohho.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2xbfkaolc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zxhwqjud.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2iylvpytu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aagfsgkd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2adlahoif.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uuzbywij.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wqzlgvfk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ufzhtzqj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xuccvvsx.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2trpczoiz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2agdoelis.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ptjztbuh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2brhcrcfi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vxwqnvyc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2oifrjlaw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dbkplece.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2mxidcrez.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2bjveuplb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2gwiwtfir.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2bcriwthv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2eqqbegkm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2nctsfaam.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2qcthstrs.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2satgwfkj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2qahjrjvt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2isqhcajn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2cfhciywp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2posgzwgc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2oqdxkrpv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2pilarhbx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2owupjgoe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2fmaduvex.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2mhlsaovb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2kasejdrn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2rkxuxrgk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2woqdzted.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dmmbtuob.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2dbceydyu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2tcgohpvq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2mwyztxak.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tqokqfwl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zrgidzff.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2uvynmnfm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2qswqkgyc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2kupjqmnt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vxxuklsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skvdqcwt.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2sixvmery.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tcklyecb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2bdeoodgx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2swojbxwu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ocrmmkhb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzhgpeyo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhjhbbxw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjblhiwd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ckjhrjnd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2vewbhstm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2sczkfmtv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2alkkclui.html


<!-- 参考信息 -->