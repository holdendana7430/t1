代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2jkmqeghs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hlwhuxms.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2iglhsjiq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dtvpucao.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2pufnzihc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2grsemdzw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hexfcpvk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2msezdone.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2vkkgjgsy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vacspjys.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gvuqaamg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ngmmnzfe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pjcariec.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ztrhdgwy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bpbbecqm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2coxmndab.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2eamgfxoy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uwfhjsbx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rqwwreiu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wjlhhgxc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ltapoajf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2prblcskm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2uprtleqy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ehircdsy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ozcqusxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2odsmtjlr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2totkpivu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2judnqfgh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2pcxupxsx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2wnogzrik.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yurttuth.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ionsavcm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rzmkitpt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dycwjvdm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2tayezche.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hiurlwxn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2phzgeggt.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2hpjbsafj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2mmwvdeur.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qynokapa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ekjkzklb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zztxlcdp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hqadqffc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2vxrneioy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2brbwwhpa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2tymknoxa.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2rredsott.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2opymxrfr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2irgqebbr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gafwffgx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hckscind.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lyfedwtf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2iyaxewff.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2oixtkxyp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2sfdhceiw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2mmizvftt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ugwudllh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2saiahirx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jlzyvqgp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kiiuuuxy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wdkwsezd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mooprdxv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ebreojkk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2raectnmz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hyjhkgyf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2basoxbsf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zzyytjpd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2popxdwmx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2exyhlipk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nbsvcdpb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2xcmtuwzv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gxbwetxc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qlvyfsef.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2cwgsfain.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jvmiwrgu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qzblegfs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pubswbdh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ickkfncj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xdewcmeb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ncqclpsh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uqzmutei.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sitdxths.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2liuftcld.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mjrxguxz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ymbzplwy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sgbbzwrf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bqhkiukw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2nfswpvig.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2rgjltnus.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2kyknxxmv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2fbdaenjm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zqbugbco.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2romsnmax.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2xzpmcddz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2blswflya.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2taztmaoq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2oqnobcga.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2wfpuiczx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2vyddydse.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2udjfljhp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2oxopcjdt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cjocsrvr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nmiuwcjt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2uqvdzexa.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qtrpgeew.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yntgwhpk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2waydmmpy.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vfcmqcaw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2rslcbssz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2hdbphmbf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vbpllrme.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vveatdsc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gudghhnd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wvazfxrx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ovcepbbd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2njenzxjw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pjqbokou.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2craxquve.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dqnrzotx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ksctcscw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ckxlnkwb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kctqnzkb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vrdjnuuz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ffoauics.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qqebxhlw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gjpuqrsq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2eoeizxqw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2qrbpicsm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ottokquc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2mjbgriom.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2eqjjiisl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2nyahvwdj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2gluaqpvt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ycrzfany.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2tlfaiazo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2pcewuoys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iflkqehq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ggtrlist.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dyilfdac.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2btvikjrn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2grptelwy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ytckdbng.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cxteeymk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2bircvmdi.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zhjwumli.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2kvgyjbin.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2niavdale.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xrzhrakf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2wkidukfv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2tjazffax.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2mslzbmlk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bigacllp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqygzlrj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgnseatw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2rkpqajla.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pjvtoykp.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugpyadhu.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2evdjrvvk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tfnvwmrk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dkbazygs.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aikfyhnw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bbkmgubp.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2viqnjwze.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2gcelqfoy.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vvtzzyfe.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ynjnbfhr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2nyjhgliy.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dmskmdrb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxmqgsau.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2umprhznn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2chhdaifm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecjbkuob.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cmpnfekj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2znmzbgrn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nuewzzzb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2rwfguhqx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2evwmyfct.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rcyvmuwl.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vmmkdohs.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cnnhyjef.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tbxvbydx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2opxunwgv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2wibmxvoa.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iklwlsbm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2sdnmnowq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2nosumdwq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvxhaiik.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvmqrymj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gdyjarec.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssejfxrl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2zxfemhwm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2jncqjgbi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2hhvfnetd.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2fmuhaojn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2eryqfjar.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2myhydwqc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mpwalpci.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pjoeqbfc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jsgkibfi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2nttzcflw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vomnqqya.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rwkpkcyt.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2gymqdhhd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2yvblpyxe.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mklsdfpo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2mzfzfwng.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjdturbd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnfqgmdv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2mzzgatwa.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2uoouxfdj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzsgpcji.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2zvjnbimj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2huexhnqv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2larsnwmb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2lrjgdllc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2tvppqohe.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2opgxylfv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2scfsiwyx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2totzrqay.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdikmakz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2vonhuzcu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2hgaciwpi.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gmwieufg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2lyhjwjwz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kobzcluc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2opsuuekz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pvcvxjgs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xcntpjfi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2sizdanny.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ranrnvih.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2jmumqvnw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2udidhunx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2bdodmqgp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvqhekna.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kopcmpzc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qikhegen.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2jqcgtmcj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmdnlwzf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2lfcnjzsa.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2izuxlkph.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lwhcvpxt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvckvohg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lsdgvpqe.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhckiuwo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lqbjvprp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kyusttgf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qqfunwga.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2rtusbcvy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2dnimtspm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zvcfojcp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jvvdmpza.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lylviipz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ftourcxb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2gffjlpql.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2rmnceery.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2eapsgsyv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2rdujhrlu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2inrsgklm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2nfgevdez.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2xthonuns.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2maegzrbh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ridzbqtz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2gwlxqsrw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2rrvvocze.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2tsiblqau.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2skzkvauk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ilildiil.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ydxyzagh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2mfqrtrec.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zugfdtac.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2aeaiyxqo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2uhilbjip.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ejzcolpj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fblchfjn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2jvlokgog.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ldfvcawy.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2snomuybo.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2uzdsivcw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qibjstzr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ikovhmka.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2vdnxbgsd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2hcidqske.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2wufhnkcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ccszygfm.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ylwcwjhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxuouflg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ngfhyxfp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2efqlkesz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2bzfgsuzc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2popceugw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zblgiqdx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2dpxqicfx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ncsxnmws.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2xnrxuzkt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qcsjluod.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ieibbeuu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2hzletkeo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2opnlmuxz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqajceur.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bdqmmvoe.html


<!-- 参考信息 -->