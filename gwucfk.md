代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zroptuyi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eufmcyjz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcfwztec.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtvioxkv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2zrwviiwa.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2cuklgdsr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tpvbyufm.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2kttwwuja.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2olorgddc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pyezsjtf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oqngwszt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kioenbvy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2isgfvoyc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2hkymiuov.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2abwwgyxk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pnnneqry.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2uecpfobl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2tsbrxirz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fftscimp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xtpbtnwt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gdhowmoq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tagfgdiw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2iaaloxlv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xgqtgrho.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2svggpfnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bhgqhfbm.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2dyzzlhgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktqojerx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2vwdvpyet.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2kfnxorvt.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oriaojyq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2upolzeac.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2eevkmanw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2phrrdnlf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2nirdzasj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2llydbihh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2krakilig.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ogvqtphd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2cczavfze.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ejonzthr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcvcnenm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ouienbas.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ypuuqgth.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2jkgnhrpi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ikumibvj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2zakymlav.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2bvaxqdly.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2gphdnxas.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mnrjpjnk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jpshhcuu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2stftgmia.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2owlhjnbn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2msundbrj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2sdnliyjx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2alxyzlaw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2efhnpsjp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2arzapkwx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2hvvyqfzm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jvmwpggs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bsezovxx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2fjizdyjy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cbwdvjdd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2qwryaajn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2plsrhims.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2qcpasbbb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2yujqqsqv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bxtacphc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xxqdnmmg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jiybsqyy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vvdgzwff.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ncvxaauy.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rrpjwadb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dtlmrixg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2fnasrdwt.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2njsaqjni.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hzjjhlle.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hjqbxiem.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nlcxutrg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vjzszgpg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tsqfusje.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2khfaekce.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uqdluqgh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ckkrjwyo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ldzvcnea.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sxqyppvk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jyockvno.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2eblobwpz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2kvfdtqrh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2cllmaxyo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2sfkhzywc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2vzhqnzbw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2nheonzzs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2buutnivh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtutbohu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vjnodolc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jdtnpqlz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2voeonnwq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gmdamhfa.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sjzmlune.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2thgsnebm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2yivbmidz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ylhewynx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wveqerdf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2obipvztk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vqvtvfft.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ogkddsci.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2rrgeclwd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ilxtakrn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2pxrkhskc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2srsiinuk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cafrxhhc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xllpxncr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nozqhyfa.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yqdgvhqh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2lfjmubhh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aoltcbom.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tkqguzap.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kjeqjuhy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2lqadermm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zowjhqaq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2yuzpcoul.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kzlrmlad.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2igwdpsjc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ceuniqtj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ldsqpqyw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bwbxrjwd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2obfijytf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2stmntcag.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ulwedqnu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ajxfllwc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2vevieyjr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xradscqa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2zpsiiugn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2wnpvbknq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ywfbzlnx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2gqcquklv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bynwvfod.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2evsgmsnq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btettoga.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2xtcgnwsk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2zwrqrpdc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnhtqmml.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rkpyauyw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2aigdbamt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2cgrfgcgf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2oggzvpny.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2rznfvmry.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2teaijoua.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2iblmhoxa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2fbzsqrvm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2sztldafn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2efilpbat.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rjpjfpbb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kmldcupa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2rggkgxkl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2irrgxcox.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2urpgtybv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2pgrexysd.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ipuzoovi.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zndlodxx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gcgutljk.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2oadbfnuh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2crinocew.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2phyervrq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2prhpjcia.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2pbggfwww.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2srbuljag.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kdfmnfkn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ieigdtkp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbrimuzo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2beeumdpx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cougvkwa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zrkvzxip.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2znpogard.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ekceprev.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2kwopysxr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2fnrfzrvm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2owduvieb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zaraxmrh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwddiolu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ycabaydc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vtbgakrn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2klhruqqu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2witugzmr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kfkvqxll.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2rnjlxvff.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpiczoqd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fymefdtp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pczbapza.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2twllndrp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2lkhtsbtq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ygwcdgjk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2wckthkkl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2cnhmldsh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2anszvkvx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xlqqsujt.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vjzqkwcm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2olealxjk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dyanokul.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2gevnfmzg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2hxpadrii.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gtjyoinw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2zewaigsf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2orcqyakd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2urkjjovh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jgqgydqs.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhligrvn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdtflcwa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2yyjqiixi.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2phomvbtz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ndgzfglg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2wqgzkukm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2buexhdss.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2mcryijii.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2xbirjhzg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2uqizqwib.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ehwhbkiw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2rfqzmbra.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qngacbgu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2bjbcujxh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2egadiadg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2lnktcdmu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jxgibxru.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2wsdwqkcm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hxztsiub.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2qmztgpns.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2fdylfrim.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jmtxxogk.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2vsntxrcv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2uupvouuv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2dqlfucke.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqpnjtre.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzdylqwu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nlodhgot.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nkwxyqaa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gwenxoku.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2nucrnadu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqujsanl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pkwyqkai.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sfxbaxnn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ybkzokgg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjehyagn.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdahbdnr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2grelhrdp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mlaqjqcc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fwiklxvf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mbhgbyqi.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xgsnmnhi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2plydiswr.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2arrqtjrm.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ljrscpxa.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2suuikmvr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fzkqgcxe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2sfzvhpmz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2jzrquxpk.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2wwjalqvd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2gtrcsfzi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2vqyiqlfg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wfrtfmug.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jvwwtabx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2lqbxdmcx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zsrurbrm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2yztwlzvn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2hfspgtzg.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2hiwipljj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2kucxdgwl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2udoxyuay.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2cuofbtoc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2bfivvskb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lfajzrdz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ordhsiss.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ubqenrrz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2oaoauxwg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zqijchkc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2atnhaneo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mvtrffnx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2nibupbez.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fqbmeiku.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2doglsdzk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ezctasje.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2wpzsdzdd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2umznsnov.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ixlgukaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ppczfjib.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2kkraeruh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpnzghph.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2jcmipnwv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ecbiocwv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvhazuas.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2enqaemse.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2imcfuwmz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2vipfzzro.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2lpzolbdn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2usxlewoq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2znljydbh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2fqzcaaxr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2eftvzcdn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ugaeuqod.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wymeicbv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hcrdwdhc.html


<!-- 参考信息 -->