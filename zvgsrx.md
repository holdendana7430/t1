代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2bnzyuqdn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2iqbgfwxz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2yopjgowf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2becrjeae.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pmaavtns.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bcrcunyc.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2grlyqpjo.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lvnsndgz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2csqoppwv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2jrsbluit.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2desnutvs.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2jqgdanby.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2phddsmly.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohllndcl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2bdewzcae.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ujnxltmt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2yvkonagg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2twkbgawz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2rzvimiqu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2iugjrfjm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2vapfsqfg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2afniitxv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ufozumjt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oaeuvqkb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bdukiqia.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zmmzhggg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bqqrsskl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xvvvqjvv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2sgpemivz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ezvlcoxx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2puarewns.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2naqtesdt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2drnfyuwy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cibmyehs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2soaagsoz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cyqxiiex.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bxkbksan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ktkyvzik.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ynupgftx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iexnblbq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2jiwqzqce.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2qvryjprz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cnheqjbg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2wvlgeurz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rguegxlo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dtycqdgf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2sezxcmmf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jglpojue.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zjqhkboa.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2kkhuqmxs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2rnlkurup.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxiqmavj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdukbscn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2olddmcvn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fyjnqjre.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ehiwnfcp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bazhnkbd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhtknyli.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2vrrddjxn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vghtmzqf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2erqdzody.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2eezhvdrd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2smqlwach.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2isrjtmcg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2qzuareoj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2okewbspa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2llexyplg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2glbqdvds.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cxaerpmt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2gcpidhtx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2thfoklbr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dcveqxxj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2iyzspjbx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mcgcvzme.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2yqoowuog.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ejfhvcid.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2axmedvcb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2loaaczpf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2adsivvdy.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tvtzmzdg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fhncllgm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2iqrtyezt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2rgnllvfs.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vndloksh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rhdvpnbw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2synrokyy.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uifzypcz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xlyczzdd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nuiccney.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hbfysksf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ahpldmbl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cmsdlmyp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mpaitfit.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jvlcngzr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2kzxeadde.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ogmgwoub.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2onvmyysa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rjvwqvfm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qoacgksl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2tiwomsve.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2wmaxqnbj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2zneivovw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2nzdglvpm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2qmcthjgw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2odeeddeh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2togtjsby.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gcdrouyf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gwzjiqzx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gwycbreo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2akfvcgva.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hmizgpjn.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2svikfvxt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2alskptpa.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kpwitlot.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qconbvnv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ismbwebw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2doijvmuo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wtfmmxaz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2fllozgti.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sgxhgavg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2zarodbmd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2bzuuuhwc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zzkguiwg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2htyzhcvt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fcvlrors.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qajivsjl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2kdehvpdt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2egigydmz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rwkegtyj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2apevfbjo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2hnvsbdhp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dzghlrrg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2etlwlusj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ezfiqqer.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ypzpjapo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ugikryae.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2myvtjlaa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eflralhl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2sccjqfqv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2nlceeojb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2qrgvknuk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2yuacqqad.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2vjvdggwc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ecqztzgu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2jsolalbh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2csamaapf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2awodtjkb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2vgnkrsqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idbbusib.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2itjwadvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2urjikvxi.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2pkbmbevo.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2rjekbsql.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2lehmlsww.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfjdurvf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxkrmhem.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2shbisync.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2udbryvor.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ozdskksh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2agybszxc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2owzruthf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2rrqjvcat.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuuvhiah.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2viebwopi.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2qexdtypf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yivdzfoc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2hzeupknz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ibakqphu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qubcmldh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2tiwjvjtr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xhnzzngx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yjlwqbmr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pyitkwoq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hajftpdl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2mrysorgk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2hrrcemvm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bzkbifos.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2mnqljavz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2zrnsnyck.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tsqxwxqm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2taubwyuk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2opjtkzwz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdvqyspv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2erbullrl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tiiazgte.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2chrdwmll.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2sznclaxu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2exgqhnfm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ctdjgmsx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2culgjkti.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwnahctb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pvppsrja.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2orvfcekh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2pebmcxwo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bxacodmn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvwqdewc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ympwmvan.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2aprxswzf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uwqoeorw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhtomkou.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkpisocy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cafsupxg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2lshybpfe.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2jkvcepif.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ivofxghl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ixzwadmu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2nltebato.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2pnltccbb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zhsvvmxf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2putjxtdz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rglctrcq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2kwgqkiqi.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2wikzmgnx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2njjbovrm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2csatxajc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2yprrtmha.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2onhqyprl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2dyflqzfd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2srepxgzz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2xtgvevqt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2umlhstcd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2cuizryoa.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2iygeotyc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2opvueezs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2wkepsrsy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2nyrqychp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2lxbjzhfh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2zetmftme.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2uhgwmmqq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ujlfetaw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2zbsicijc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2semhslcj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2lasdsska.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ohgysrov.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mxrtfcnr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2lwnfwzzo.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cimzbmcr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jpivqrsj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2wcilkuei.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2oiemkyvb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2cbvjsnad.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ezvtzmpn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2hzczkoes.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cojrjdhr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgztqsuw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxdcadhx.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvztirkj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qqhkcvqs.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2oywemcrj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2fkdugnfp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2paazrhgu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2utzapmav.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2odidclne.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2doerlzgr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dzeuhwjg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcynyqwg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2covcwkaq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jyeuejws.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2djbfavsr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2iaaolwyw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2iqymgwra.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ozzipyms.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cncfvfvq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2thfsfgtp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wntlkodu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zuajlfid.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2miketdqo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2idbnljvd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2uekydsta.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2jbxgnorv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2vxipfgyr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2whmifqhl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2zustalsh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvtzjgeh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2bcldxdnn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2tqnjyesx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2bqvkewcq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2aifplxru.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vjhfogdx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2qljblguh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2noiniyri.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wnshnrug.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2xifojfdc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2pekyosgq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2rainfzvh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kgcmosbb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2mygthjqs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2rnfsvddj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2bneegvmr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tdgsqses.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wnfpedtp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2drfkjhkb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2gpnparlk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2egaerivv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xheainxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yegmbvsc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2qmqmrbcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wxofhqyf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2pczvgncd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cokczrxi.html


<!-- 参考信息 -->