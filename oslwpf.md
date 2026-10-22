代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2akeqntno.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2oyjicvcx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pouexigy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dourusul.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2oqaefnuw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oxmkvqpe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2duxweeho.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eitcedss.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iutexpcc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2urvtcusr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2okjwtpoa.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vsnlxrii.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2klktkzly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqozvltg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2iylmamou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gfrojvwb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2fluffohy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2vabbkcpt.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xgchvsig.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2audlhmpp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vchjaipy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fpybbtkh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2dyahdito.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lrpqpbsw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lxtecpim.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2tjxegfqs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2bjlpsfni.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvytikcu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrauygew.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzeswvqe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qafftxip.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2zzeupfch.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2uderebqr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ohukbspq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ggbmhgam.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2xysodguf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nocilrhk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wvihycbm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2stzncbsj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bjvvbiwb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ebrgqesv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2hohmlzph.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wtgcqxie.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2lklaqnlp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2nngalogd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2yiyzvpmu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gppibvmq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ygfltvsa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2akfzqyze.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2swbgjfxk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2xkuqivke.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2fbpntgpw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2bxuvnzva.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2lgpginur.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2idmwwhhx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nvldzfkc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dsleoncn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vnknvifg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2opmutiie.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gzsauwaf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2udzgsnmx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2fhqwnpxi.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bekagueh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fnsquxca.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dvnyjpcy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vduaivmk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rgigrxgm.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bweqmqkc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iftjxson.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cfpengfh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2kyfkyqvu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2atstabqr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tqwjmovi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wbuhwhbj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2oelbstqi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2crtcokfa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2fbqsekim.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2dtnstule.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2dkhuzemi.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2dpazkils.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lyjhdghq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2orhcmcrr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2uvmcrgjc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2juwxhfqz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2whujauey.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oqjuqtww.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mmopwgjw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mnrabdrx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ynbmzblr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nmownzcm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2itpxjueh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2taqavgra.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zqvdlpve.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zsntcjfj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2tslagkyi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjotpzje.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2dkyahodt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ysxrxqgm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lipmbtvp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lizoiifc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dmoaekah.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2twxzamci.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2qzkryiev.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2urtbkmtv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lvauubqz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nmupvseq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ozxvnmel.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qardfdyz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2pipvjjep.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lvuwktwz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2flnmmduh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mkjdfzsr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2sejxmwny.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jclwbise.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2lrlxqccu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2jsawkotm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2eokvutri.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2qztornxk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qofkrhds.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vvlwstmw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2izqyjxwz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2cdnzbqkx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2rnmuetip.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2wtwdjbcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otnrdkaw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2gnqjqjtl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nyqhrfpz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2smdbaoeh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rjjcrmji.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtkcgnmu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cuebkphz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvdwlaqf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qqcayjkv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2sppytpxp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2slgtrasc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rczflveg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zjkrxrgr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2sywrrsgq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxvcpygc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhpvofxs.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2eysthtbq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ytvgzsbi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2fgkncnlk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2kijorrap.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fsckhklh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2msjzqxba.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qutscwag.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ffsiwhlj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xsnwyjvn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2iitzqgth.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2lkykjnfd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2wekaduga.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xgicmlya.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ihcfhfwy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2rjnatamt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2pvzquqzc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqxttiev.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2inykrgwk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnsxzeas.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vcjzqinq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2islfhugy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vplfbjvd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rtdpiifh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2fsjcrfpp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2niyrxoxi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hamkxptr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqfhuqnt.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvfxiwnd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfxwkjyy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ugrdiuvw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wmuprwiw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2dlpkisbb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2udcqakdb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2qghslidi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gksimaaq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gcuorbnc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsxjysog.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyuxbrfg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nqlxjxil.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2omxbnoaq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ttjttmsi.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2lwthiozm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2pllphaqt.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cvgyijtw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hkukkoha.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2adseriet.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jkjtymty.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2clgkcxiw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2kacedlgx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rtoexxcw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2eezmrhwb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2pcurqryz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2fdezpxms.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ienckkdt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2pnabfcvs.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vycbjtyx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2zjnsfxuj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2rzmcwqzc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2chktxouv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2cffpzegz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2qbgxspgu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ojeagwsp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2rrubrwkd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ieqcqyoq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eddjidoc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ybgrzyvz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2gcajzvqd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iuxypuhn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2rgackkew.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2itnkuixg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rnprclyg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2jzovhobi.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bustzevm.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ppuohobk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pocptiov.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xzerrknx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2nmpjdalq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2hfpbxxnm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ujrshksm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2utnxzzcq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsclzbpa.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgvydzse.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2usgbrnub.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dcyhypek.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2zbtsgiqj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzgpiuof.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ocaatcdw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sfpgqdsb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wbmcklkt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksqjqqeh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dobukubj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tfdaftzs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tuyxfkco.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fatwuzkg.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ppfikvie.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ctldbrpu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2sqnmbssa.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nhozglra.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2doizvher.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gyqazwcg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lavkkuww.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2vrckimgn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2oauqmotq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2cgrstjug.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2laypdadz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ahzkfqtw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2gubfdiqe.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2gvuhwbtl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2crwqfynh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ldiqyrtv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2wcnuiuny.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2rxexddmr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2oaaasfyx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ejwfnxig.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2zymmimqb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2cwmcomvq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2gwrqawpl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qevolwvq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2qdjvopcs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2sdnhldwo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2iurqljza.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bpssqsbq.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2vaokkyfx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2zahhhjdl.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2pewoqkzs.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hobsmoyo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yiedknsz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2idrmcyza.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2rlvefcno.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2olnjtwod.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zlisueno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvdyxuco.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2rfdkfkny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdjrfnxw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2liagcmwm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2radmgcrs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdzxktuc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xotdxblp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2apviimmm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ijrjehqy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2mimsllof.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2jmfrkswq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2doffspvu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2mdpjdurd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2bbxxwalv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aclepstt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iiinukuw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rnmtjdhx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2quduxwti.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2cbzgxvui.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2xbwilwbs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2juotoakj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wvnuqiun.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2nllnnwve.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kccaxxus.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2srktyqyl.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rrgaumbc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2htknxbon.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ohtkiwrh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2wytavkfz.html


<!-- 参考信息 -->