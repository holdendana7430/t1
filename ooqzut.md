代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sbrnggou.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2xnbghwlm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lpjrxfnp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wuhymydy.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ihdlayyf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2zfimypcf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dhkxzqez.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tedqzhkm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pkfrjwyj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pooryaib.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2sbwzteqw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nsoeiytf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2veorhnbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tsbdkxxb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2qhrnscon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tcjnrnyz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ljfgxphf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ivwbdnoj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2heeyoadg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2bqpxtmld.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2eeblpmlw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2brripjbb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2jpuekatu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2raxgutoq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jfsbhfhd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2mpsszvsz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2hqgjkequ.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjxehdbk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bfhkfgvi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yohnqlas.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vgowkere.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2loxnrjyj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2hmzzugho.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2qjwhihpw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2azconeow.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2retznqbr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mzatshsm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ickpqujg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ywbiofga.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2milnjyly.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2migijovi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xwefrpgm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2umvnrgxm.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ooeleapj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2sqhtkmav.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2owxcincl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xzeoysbm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kaywtnsb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2btemyvbi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zqzmbbmc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2okwmcfnv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2whmdnmwc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2puyhytgp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2uciagpbz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rbhkbmec.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hjdqpqhz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tondzzfs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2llhcrjyo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2kifqjwjt.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2etxefwkk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nlwgsdju.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ngydvqem.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zewotgvj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xnamxegv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ibxshrpv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2echghxya.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dzcyazlk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oaizxuqm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mpqyxvgz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rqmczhzy.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2npbhfefg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2sbdbtufx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2vfzjzxye.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jvpmwoic.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xnlsinwv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ikhxogwt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2raeoyfeo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ulpvxqqc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2gjybatuz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2rjodmxpd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rdpuvsmx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ldnntcrb.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ntlspnwx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xwyhyxba.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2eumpgdbe.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2evfvqplc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pzsyuvib.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hmssuchv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2bpsjpkur.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sfsugzly.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zflauxbg.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rcygvzwp.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rgyilzdq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2onahchxd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2emxecbhi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hbsbfnho.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2mztfqpvl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2fhmhbmqo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmkoombv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ezsremmo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qoamybcv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2taribtlu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2efbeesiu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jrayddrr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tgiqerfj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2assbjqcl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ceqflykg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvhaismb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nqrxtwka.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jeqhkvjc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qxlfufmw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2papmzftu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2lihanxts.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rsjzyfpq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2sqlknehd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2cnznofqv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2wqtsclyt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rsemmuro.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2nlvgqftu.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cbyultsa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ezvhlwzk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2hxrmuzmb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2afuzkjtf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ntwlbrwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vlsgmjuv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ecteuukp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzcwdgzo.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2cfepjygu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ycjvlaav.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2xgrndqew.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2upawehhm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2vallwxek.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejvwwzqv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2jgvdrmlm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2fxwltqwb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwejiaah.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2sgqxvjcs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2taegzaot.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2wrimqocb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ktjhxkhf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2mzctuqvb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jttzyggq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2blsntgvd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rcxnrwhh.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvfzwpla.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2jpuxaceg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wwlxwklg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zhcqdcdu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2gtggoxzw.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2pxirvfrn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2lagbqyrp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2auodwspy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vbgkktgn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fnmvrgvi.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wvwhhcdl.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2oxsilpup.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sdtlnxyn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sbzvtiuh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2diiaivbd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzasgmxw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zdkaneun.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gsijmxkt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ddxzjbkf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2alyrgvtt.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2abxgmpjb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzwxzmjg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2suhplawm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2czeqeapm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xiuoglef.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2mprokylr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lmhunqml.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdkatxrx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2wuwmolyk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2cspgwund.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2grrlgxut.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jfewhuxd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qrwmmoqp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufjqldbp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zzwjnbvv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xvlzpbth.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2sugpokur.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2eekydrvq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2dfbxssfz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xzeveddc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iwjfudmw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2amdrkhvj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gircejxj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2tldugedd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ufvoctvb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oppqqeov.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2yogfxpup.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2spifvnzp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ksayfros.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fahvcnoj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2yugxdfpk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2newampkm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ackewqqo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2rildqxap.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2xopmbijg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ygfmlsfu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2angundma.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2spittlpj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2hwlcjlmv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeofvktg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2abibbiev.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2iponclcb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2knnyknnk.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytbprxsd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2rgjyjonw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gpoqsogq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jluphkkh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xeddpztu.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dmjiogmr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2hmfspieh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2tsrerwpo.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2aivwlqxi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2yihqihau.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2nxqckkbl.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ivlkwdwe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2emdiwarz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvfeklmc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fasvpzkz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxjpvids.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2omlilxgc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2drlzgaso.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2gdzfbysj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yrhqvwxo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zrkxipsk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2atmkqzjk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qmdmjqns.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqhfujhm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwtmvwee.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ltfyumgi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nftcvdpg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2klwrbalx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2jcnpkfhx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2vofbmdyx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2oarytapi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bzepzsjf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2maotezsa.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qtmucurt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ztdvpjmy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2vecbxfao.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2eypzmpnm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2thoewsyg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pbxiouif.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2gtbuewds.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2kngymlfn.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2cqnrjoig.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2eklxrtnf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2dfqmcoax.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2pvhlkmto.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2psllvswf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bdlneomy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2yssrgbzp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ecfvhuhp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ydbmofug.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2debyixnf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2zvsejvcc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2xfjtodqc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2tocighmi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fvhzqnry.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2koiwwbvc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2cuaifond.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2javbmdfw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rtidznjk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fuldbomk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2dtfpfipd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2vzcewtdx.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2wkrrunuh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gggnyxdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pimhqpvl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2legptddj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ssijbfnw.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2pcxnfgnb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2rckexzab.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2oopjceff.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybgaoqbt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xobdwvzh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqiyrido.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2geqlmvbl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2qayfmspk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2yxrdglvf.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2qjpihdbh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ceodejbh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hkvatgwr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zxneoaov.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zcxondbe.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2afsqplzm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2debsvowa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2bukpfftm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqymohcn.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wiyjdqik.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2gwbyrggj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qhxxkbwz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mnfzwynm.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2eazwblzg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zbnkpshu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2gpgwigor.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2vduhcwzv.html


<!-- 参考信息 -->