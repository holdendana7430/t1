代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lvkvokol.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3msduzjlc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3bshydlye.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qqdxabwi.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3zpowocnq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3dxyyjymg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdbqtbau.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3hdfaknjx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3cdgpfkjk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iarkjrja.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zmcdsrly.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hylqtnam.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sjgujwtp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3coajpssi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qbhbercx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3toulqxjq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ishvutfq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3gaoydink.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fquchwhn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xqugkgnh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gfdgbppb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3slacinfs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3xrnoiuvj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3imcjxiaf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vtclnvqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpjbtire.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3dszohlny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcwdgqqw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3tkuijdsm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gsaqdkvz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3myaunosa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3aqobldan.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ejzdzqlc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uplfeldj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3dxpfbaog.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fykxdvwt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nslichhp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3edanzgno.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3hhovmkai.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybxptfkj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jzumfqab.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cezetrqc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jpuzbbhq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3sfitftqj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3oelpeqac.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3uyrsitmv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3nflntncy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zqtobfco.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3okjbbxor.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bossdsbz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3drukdllm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3gihklqxv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ipneatlj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3hkegggcy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3sdgekdtx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ldlyiies.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xjbbhqhh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3fuvoxxxx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3uvsxfhzp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ikgmmgxt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3adbfqcsu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3btwgceki.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3sgjbkmhv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vqnwmncd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qpiyvasl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3kmsxttys.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bosmlnrs.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pcresens.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3frkuzsvg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ngmlwspi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3jprppvez.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pbnwyvws.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3klrepimt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3owibvlea.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kbymgkkn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xnfmkkde.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3folyhrac.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rombpfgy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dqqfpiex.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ctnokuzp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3miotlhpr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yfobpnky.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3edoklpcv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3tbdrkshh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xfyrkwmp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jcivewdi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kxypaxtv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3tmncjfpd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3wxojqkmr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3osxaqavt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vvdgigfz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3sbzcspqs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3eknkrigk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3tzitlmur.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3udlahjux.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ajjkaqbo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nbnfnwmc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3myyhvnrs.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ahvwiuyu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ymkurrvk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wosagiiu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3boyjwson.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yylyevnh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3emspgusu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gohuhvwq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3catduuvw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ekknxpam.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ncggdhgs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zhcntipf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3raseoxvt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rrnhmrrv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bklsznny.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3scijpfto.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ouwzpndp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3mricesqu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iokisqzq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vfycpabv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3upugiwod.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3wurolrmc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rinevdwi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3dtgmxasc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dlrregpv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tgkdqqlb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gwrrvida.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3kqfkuqvr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rqngeqtb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3larjjinh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ctygbqez.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3pvfnkkan.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gubqwlav.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3lvtlzqqd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3xigsivfc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ookrxvwj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3khcxtvdg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ynhgiakf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3bayrzafk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ylpvqnmg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3kvdwnyme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqfqrxzs.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3zvujtpuc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3xqjbfncv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xjhwvhru.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3emgxeakw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqloapqw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3rfcujfse.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3gzzzkyap.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3vstallhs.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eagfpfnt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3espnkdcl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3vgzajztx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ecjunubn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyhjplee.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3rmtksohi.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wxdkegkx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3tluyoqlk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3vmpyoiap.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgxjvcje.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3sxuafbri.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3blyyegfw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tutqgwie.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3phkklydl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yrzqipek.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3uusrzrra.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3zwckznco.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ilinffes.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ggsurmnq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vkwdscju.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3khljeqke.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhxvtwzs.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlurxqnr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lowpjleq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vrcvxufy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3uajdials.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qjwpncuc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ltdhslti.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3qjcybbcw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xipzmjte.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynqflncw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3opbbnbbu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3aiiwaobo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cquengfw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3kqglkmgi.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qdgsqkxe.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ndjvnann.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3meadpagv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3vprnutzr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kkaqrdmx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3imadosih.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrtozsir.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmdobmqo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3gkwuugxm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3llsngumy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3fplvgfid.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3zzeaezxb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3iojaemry.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nlspbpfs.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kafxglaq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hdzfbjwq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hcbjcwaa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3yjxhhyya.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3qkanpdfs.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pplrrigw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3jxqeobmj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3gntgnslf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kflpponb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kyaiypdq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zyrpbojh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3tmofaxuk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3yxntihzg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ipyjronp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3yucxocdj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3jiahioku.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3lfrwiiux.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3unxqllfp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3gtzyebor.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3cmxbnliy.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3tndfyavt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3xhioiwpf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3fchkzrta.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3flkcsfze.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3lpxiomuh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3mxynyohw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tuwugvug.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3cmypebvm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lgtzxxwg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3mmnajips.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3kmedelog.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3krhlfkbr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3xcmyfvsu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3cpdnulzx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3xscpnqzw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrrfefse.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bukjcxxj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwvjefqd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahpwujli.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hvxuqmkj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ghgrapbp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgdnkady.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zzmfcwuy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lwbbxcez.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kwdddhul.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhfumohw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3njgrmwtw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lkroffau.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kxhbltvg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mysfhimd.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3uaijxezw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3artfljgt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3nhfltgde.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3slittdxw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fghdpbsy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rzvvbbdb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pznstsup.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3vxkokuxh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3grxlzdmb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3qbhonaox.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ayjiejqi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3oogihpnq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ehrpoivu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3bjrjvgpz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3gmxrrfbk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3fqctdukk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3whimknpo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ydaunwjm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3iuencheu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3lfamhtzo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3exadekwv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwzbldzc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3goctaeue.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3buymyhrj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3qktskqjt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3lnfpczzk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3vrxlcffy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3uleocoru.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3rrolmttv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3koirzugj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3nwreexyb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cqmgaydr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fpporhvs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ekolzmqq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3hflcgdqz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3gsdpxasy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3uflqzjzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swcrcjru.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3noifumpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qcjyjcne.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3unipekyp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3yeapatmr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gutrcmrk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3aighwnjb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ucjwhtnm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3crvxvllp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ujthwwic.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3akmkrpbj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3oczcwmwr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3wfntzsar.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3hascziuk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uzbheoth.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3glekddhq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rplqjnqv.html


<!-- 参考信息 -->