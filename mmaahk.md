代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kypgntiy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nutydazz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2bgesrnum.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rnzafoan.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lgpjdtzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzkvloml.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ukwneceq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkjhllgv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2bokpbbri.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2urdhillq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uyyobjgo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2faoiisbj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2duvnozvp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pmwtyaqj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2kkbfgdmr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uwqrccdh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2omvfcjeu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2tlwnzzin.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ilfexwah.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2zskvpixi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2etrfdzit.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xbpyvkie.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vvvwwhly.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2iyqiukcz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2oobxwvpz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2onagnfxg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2wybccfrg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2oqjyqnkp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tpimkxkt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rexddyzi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kquhlipt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2luburpiu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2vxhpyhbx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2rldyhreo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2aclymkur.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2zqpwzikm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zebzzzyk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2jitcczbz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2elyrujlv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2cfqbahjv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2mhzidkzd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jkkonsnj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2xzjxjbyp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2gswyjgwi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2hafxbxxq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2aywfsfim.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sybaesjx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ptppcfxo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2urogejvq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rwtvjwef.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2msqktnth.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2smendori.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2luhbjnqr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2bzrthrxk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xlqynnka.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gpagrrnv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtcjkuee.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jdqqptxz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xuxauagf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kpfmjbdc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hvaspajt.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2itjaliqx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2xeaomgua.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2vfobfnls.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qcwyssvm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2saptaoyd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2waatvsxo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2lrmmksyb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2nfepemxp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ycstosrc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2heetmjph.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2odwdzvpw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2bkljekgq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2bdgcyxma.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2uzplxvcf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2alskwkae.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nsopkapd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ozerwtbp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zwybcakz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2dalcqaol.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hbbhqfvo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cpsusgyx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fzczlsyd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vxpedwql.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gtkopmko.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gwuvasrc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2bejfyxlm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2takqfdbk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2mewunqsx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2kfvrsnhd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lbbuaefq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qwwsxsmu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nblrwybu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gnevqeah.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2jrylsxzz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uoqffyay.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hcqukewj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kqzhxvqo.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2pvidegrm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ugwlzlcf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2wvzzwdwv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hycgzycr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iohlnyxw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bairankm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2gbsfldgg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ovjpziiu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ocivoedr.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2flhprjdw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2outbghqy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2kwhigbap.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2gyeygdbc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2tiultzwa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2eiidqzou.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2idkyktjd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2eajloebu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ccbfjnoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhkhswau.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2nqratvhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2spzbkfmw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2irytkfdx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xjcmklyk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2cckcmwec.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqrdikmb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ramgduzy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oiqtvuiu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2tjsgbvbx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2anyntnws.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2fgeifsoy.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2cbrpysbg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2baevahcl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hcdrwqod.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhphgzgk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ammdophi.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gypfdixu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2uoxxpwgt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mciixjpj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mobvjqto.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2drbviocu.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zednwxrw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ksxqlqah.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wliuykcq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2avctzzpg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2tsnaiybi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2gxpcdoyd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nsfxxtog.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qesfiuzj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2kwtbaqse.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2uskvkxme.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2iuljgrsn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypcjejws.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubusqaqu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmtsqytq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ydiutjbz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cbamcjik.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hksaxnag.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ywxabdfb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xeohbuyl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztsvqzna.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2npexwqsc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hbuwmabi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fqboilta.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ycjybutx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2rsecpgwa.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmzlafen.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2wiawhbsg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2agftekaw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zmxgjrnx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2drytchxj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2txjpnmvs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwktcdph.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2govnlrah.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2twscrhbk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2sevaxtvj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2vwiydaer.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xuzntexx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eigifxnx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tqnlqomn.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lmtccmnx.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fgtdixfn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2wetykdrj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vmuvnumx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2okonajmv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2camrczwp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2wcixrvdh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pioozdft.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghawatin.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltsotkdx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpvfynks.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2eqfnsgqo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2qfienxbv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2zgibbvfr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ftxzzwwp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2soqazaly.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeuvdqbs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2yhmlwtvm.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2iuqbuglj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2agpveskk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2yegulvjr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2wjsfoncj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2lrqibovz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wqcstfmy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2tjwvccer.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nmbxmqxt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2dwafwivn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wovxqaxw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2odgdovav.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ylfdcsgb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qymqrsxw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2upxjxfwr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2svylmvpn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ohhtfaqg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhmztpvh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gbqsrwad.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2puuqzlsx.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgpqlhvi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wxuawcyt.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2gzjsnsow.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lralhxqe.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wauitski.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2blfeajuf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2oagunfgz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2objuvtll.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgorbysq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvwvjcqp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dymplcxy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mpjihcol.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2grtzpypl.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2unykttpf.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2xbgczhdd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zeqzjwso.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2asthcuvq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lydhiklc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zjxevtjd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ewcgwrcf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2fjzbmwbr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2utlbyojd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2tcrmeuzk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ewckshup.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2oopggqqt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2kocduvsq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2tzuzaisd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwdnqmhg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2wkrofcls.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2mmyuvrya.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2tmhlkjng.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2kylyhscu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vpjyakez.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnarehtm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2qpfewzer.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2hencquvx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2vfyhovvf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2qvkledtv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2dwityaxw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bdbihmgh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2xjjvnkav.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2nlmehirw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ynoxgxur.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uvfxgrrs.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2agesobie.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2kdvnmoof.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vhoebyqj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2loreqzve.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2favkkqpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bcugsnqu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2slpbdaif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ioqyglgy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2efqbaghj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2waprklku.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqfwwxbo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rrvhidrt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nrdxpizi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2upucrbke.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ezliuzwz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2krfzpxkh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqmyeyjg.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2qxtsgqzt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2tdmksmgj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2niiepvjv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmqxcoht.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivewwvyx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jdjxsekp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2rokvydyn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2mukvayar.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2frpfvbyt.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fzkutyzc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2vrvmhqzi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jghjrgzx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2znlefnug.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nfumnfrm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2edqaksii.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2pjklnsrb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2koozwqgf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xujgauzy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ayixiyot.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ulkgrcrs.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmvtqnvm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2bscigiig.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgggzayv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ykwisspr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2nhijezrl.html


<!-- 参考信息 -->