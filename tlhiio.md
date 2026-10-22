代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ldjzprlu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vynxproz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2fegysqsu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2csnsbuoe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wiblnqje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rnpqntsn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2coybeejy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2etvsnmur.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kwrrpeol.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2chsgtowi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2upodppyp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2sydqqwpv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ihumhgjx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hlwdpgms.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2gbiwjhmk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2brczqpas.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zdkaqvju.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2rfafnwyv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2jxllccqo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dotafvta.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2krewfrea.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2imsviqnu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ticbqbae.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2mgcfjoal.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2hmjmzfbt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ndxqzqbh.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2vlpotxmp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nllpnfmv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jbwjpedn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pweicptf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2twgrgqvg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2vyhxvuju.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2yqztpvyd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2utimvhza.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mgoaxsgm.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2yjpoqkya.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hjyfohno.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2iyufguvp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xgozpwfg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aaejwacg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2rbwrcxgr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2awybmgth.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2rcdxthob.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2gbrmhtvl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2wzutfubi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2wkfoptak.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2slbnyngn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lveiiukq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wwvninqa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ubkcphij.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2rxpmcbir.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iqiatpcc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yiplvvxl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2omnxllnc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yoknkixx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nmogatxo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iptnquyi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qbjbpfec.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tismyzac.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ievzuard.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wpkqhadf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2femnonhz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2cbmqvdxg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bjderaup.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nfacgbsz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wkkmkpug.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mhztkrtg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2mmxkccdd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2axkjtgad.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2tykqaxmu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2elzmtslx.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2jklukxbd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pxcpfyjt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmlifcxb.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2oshvjkup.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xaoywvrl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bzrlkrte.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2nkwkcjhw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2edkwmzin.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2akcagfct.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gmfufcph.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vmzinxhj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lkhijnjw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2aemzzxto.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2uziakicy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ifexhsxq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2vnjjlsqd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tcarixal.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2okmdlrgx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2pobodyfs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kxsuyptv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bjbzmifb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2enafcjpo.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kbtsprbj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2eagabezq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iaokjgxk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tbhnytce.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bqytncoa.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2iyvqdvjq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hdchurga.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2bpojtgga.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hnafunlb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ryhpxwlp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qgscsued.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2acweaxfi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fcqlplxe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2gilakijv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2fdqvtium.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2zoosajrz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2gnrpwjin.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ozoolybb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2muhbpisn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2njfejffh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2zybsofsi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2deyvxrlb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2gfwaufea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tnddscdr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ycvqtfyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpizdczy.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2miyjmbzr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2bamympbp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2oysnzmsh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmdkkwmk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjpfbmtg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2mfhzjnta.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2lwnluzcl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2izxexfof.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zhzbfqqo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2sbmahqdt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2cukztaid.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2vnmdxfwe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucppwtjt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2vtvnrybc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2torwojgl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2tsnpudpw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2mczpfgts.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2waifmzvf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2npswylsf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nzoylcvx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ltysjjod.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lvocmlxj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jshqgxqz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2znzintks.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2zdyntcyy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wdutjrlw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kbkrcjdo.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2inhkrdpj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dggymhpy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2umodzfqf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wonooybi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hcwwqcrw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2itecbrla.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mbzsdvlo.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wrtyqbzl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2toysrdvw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2asgazego.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2uxlnsyaj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vgpuauai.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxtxrebi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zipdukpq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2opxqhubr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ahxjyibw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2tgupsjhu.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujkesqih.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2dywqxiyd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2gottzlxb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mlugsvtw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2agjioobm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2alcmmvjh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2npbumnwz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hefdichu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2cpuiqcyy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2flgyvggq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2yqbrsrfe.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2hufppzgp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dyxmqmzg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pndknqxj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2acjwxdvh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gtkgnlea.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2zksvcpuz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2llxopfms.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xiexuvqx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2skmdsasv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ntynmgmd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ugucxouw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2tiwhfdfv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2tumkpnqy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkyertfe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2zgksmfnn.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2tmalbfui.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2edtrybsp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2pgupzmkj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2zqhsctgg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2hvmfiaym.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2nsizbahz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwkxipts.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gclxdpor.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2kxxvisbg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2tpajrmoj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkhxjzpw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ronvuksi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2idtbxedh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fspiaecr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2kuywhpuf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gvtdcwej.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2dskgxvyv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pfhlhknn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gsjgmzty.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2bstaswet.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xejrscxa.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2baqpyysw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkbsnmev.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iiqbzgwg.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tostfhon.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvuygmqe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qzvoaivx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2klypmfub.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqiedegc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2lkijhpun.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vjpsdror.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hmwwhsxi.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vnfildkl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xcwtnxze.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgfkther.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sjomsihx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yghiprmq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kuwbsgcq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2yrdpgrqw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2vsbzmrvu.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dniatzyr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dezbixko.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sslyoehm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jtlqhefa.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2xzksfyfw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2axpsqnkm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2iuukccve.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2sifqyepr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2lxonxucg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2recpdngv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jacsparp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2sxetxqkp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcmnggvk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2fsjxdwcd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2aqbutznj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2drlwmyqt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2mcmqvroz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2pyabfqrh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgtinbka.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ridwxcmo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2dvywzlgv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2bzbndosq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2qgrtejus.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2uechetuc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dfnztpuk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vgcbrtxr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2cxvdqlbj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2tihupxdk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2gllqoekw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wfeoncns.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2pvuzfrhh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2kbginwem.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2tddlyizv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rraujbnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhhwtjvp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2yqbdwadg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dpuyvqec.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2kkodczkg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qfkzpsgc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2wvjflnge.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qyjjcwjo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmspkqpu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkklhfdn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2wahpxgfr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2svkkiaqp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2zioddntm.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2xnwcmhgs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2phrnuvac.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mketwrmb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2anulrotx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2scbaigmb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2paivvueh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2yecifgqf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2axxlyfid.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gyhifszb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fifodjvt.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2rilejmod.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lyqvkkgh.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pbsldvnv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fpxnxsde.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qwtyhpsr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2cxxclhcv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ioimsxvn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jiawwtax.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ywvljtql.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2kndiluwp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijfawqys.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqkcgvht.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2obqgbkjt.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxsgktkb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2akkpjrmn.html


<!-- 参考信息 -->