代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bslwerag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijpunibf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2fgqprkqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wcqbihjr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tczjkjeu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ngrvhbhu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jhjwxrmu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2qottdhbz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zsjdhnyq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2geiavkzw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2noglszpt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aimtjlbz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cfogutgr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2fjpdhtqu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jlorfvzt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2timfumjy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdqcnypq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lkleqmjm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2iuzknzaa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2esetycfl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2zbkxiutz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2kheywmbq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2qhyvsdbc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gdohsolk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2etllfhsy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jidbvomu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yegvsscs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2yswokpfm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ghqrtwli.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rbyexeiw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2pdgfpdni.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2phwbyaev.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qszsqayg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2tatntxpn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zxwsqxnz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2tfmmaygy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2mmypaftx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2isrdaerz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2djgjayvi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wxmtpkzm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2wlwhoakl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2uxylsgai.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rauqheir.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xdaorvgo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pmepbhqz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vmlauqce.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2lkqcfmtv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cvwalwpd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zhvyeqds.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2zxysdtxb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ymssvzfc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vheymzsz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zcehhdpp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqyqbqhx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vfvbklru.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mxamtghx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2isdzvbgv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ersygouz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2loqbjzxl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ezzuvcjg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ttelmara.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rzoljvxm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zwbneyvo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2mscmqajy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2qcssbays.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2pnuzqwsg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2qhqampfu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2kugcrqug.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2oktzgyky.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2rbjkqjbr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bcwuxeba.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pugzubyt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lypqtrib.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ewqbknmi.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2lnyyjypj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uijjoubf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wgxrihtz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aiipjgjz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2btwpbiwx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2djyswfit.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kixbwoob.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fyjkvhnh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2kmgwdyye.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ntldfzqr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2nkrekwbl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2opmbtjhh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2unhiseha.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mxsyansi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lhyzweso.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ftzwcpac.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2cpsxfpby.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ykxgluem.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2isdhxmly.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zimzyjga.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2wpsxvahj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kfeqyfxd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zibvudyt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wplbxcan.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oambhuyl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wxszsqlf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ontdizhh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2unhcevey.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2qrvbgroc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2gplwtvdf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2mzupavzc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2gelghypo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2nanvtpoo.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2gabbfywt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2nxywmtcl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2oqsobkob.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2fkicillu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2xrjavbqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfzhzpep.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2mcyyfyts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gegufdds.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2mfglmmql.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2doakabxw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2jlpdlkev.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2sqhrrpar.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzfefbhu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2edtxpsar.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2cyxaplug.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jwdtawex.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqdqrqln.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2orjekasu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wshkvxkw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2qzobucgs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghrhpkri.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2tlmaqwrl.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqfyldeg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2wqyabcuo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2jelomfvz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qujmolzd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2pgjvhsmm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2drjlegqb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2agsvpbpb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mvqymlos.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2imcburfq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2opyovpee.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2jwthfzrk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hiuuaerr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2wwtrbbwa.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jhejcizs.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rfjfxqyr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2inhuxqiw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpjlkakv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lobluhjt.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2arpsesjd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lqjllkeb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fmwanqsz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2aaepfqua.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2hyclxigh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2qqheytpf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2snpjpaxt.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ukrpigqq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sibtycjw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2szdmnqre.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2yqolomsn.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vvjoejtm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2mmpczvdb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2sspfxivh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2wsemhfsd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ouqmfjex.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nzqnscdi.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytibeofh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2evoytlnn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2scnccfun.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2hmarcjpk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2pvnogbsj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2zffruuvo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xsnpuhkt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2kcaylhlw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qmcohpxg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vcilmrrv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ruhfjpat.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2zcjcrden.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2wjmlczmz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2msaserja.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2slnafgzq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2daitexjk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2opmroezn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbxzvtpa.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkchdacl.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2lhdquxzl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2dcyhnuye.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2mooymmqv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2oqzeqmlk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2cozxvwpd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2xobooybb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2eeuexrmk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2jpwmixnq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2gpaohvap.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2emgyigpx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2wuqbiofe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2hxqzwban.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfjjnplb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2sujugdah.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2lhjfzufm.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gsimzwqz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2yuohgaop.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2htoqvupi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2bdkbqghf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2wdjtncxe.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dpvtvxjk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2oqnvgcvs.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2lribkdhy.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2xajjldef.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gefdzaqw.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fclmdrfb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2woorsnpo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eqevsfbg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hutdgeie.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zihxinfd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2onvadvdl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ckhasrdy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lvbdsjpu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zvowkhqm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2javffetd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2srrbfrcm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2afqyjpqs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2iseudrpp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pwqhgufd.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cbdjqpqj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2zkjkhast.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rzwspsls.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tyhdqfos.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cwiroxwz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2psmdmdkn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hoxakrir.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2wtfcvjpp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2uetpemmf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2cfjdcuoy.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2yzfjejgx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2uttyyinn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2sxcoabmd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2dsxdvymj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2lzhpuvzs.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2azywubpa.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2rkukkclu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zayasmwc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2xtynehep.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wvraaihn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jbutrerw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2dkratuvb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2mlsfdwhx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kredbtrq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2acvfmslt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2qhceunba.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2mgdzjmws.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cbnfhygw.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2jjkhywdg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mlfseday.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2jaqgalnc.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ihxrethu.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zseevyya.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2hhfqndge.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2oeeihukm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2sfhkwpfe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mlphwawe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzkonaip.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2suearkvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzylfbns.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2wuulunvg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ysxtbaqp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vaeuxttd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2urhrqlvg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ucrjdkof.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2aqqunlsk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ladriyfb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2koozdmsy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2xvifrjsa.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2vaeqfshy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2seipfwkw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdtbeqph.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rzpfupej.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2soklwpcl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2svmzvrbi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2vfbbyihr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2fujlmsgq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhvacvgj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2uiczkxyi.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2kczatcha.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ureoubjt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xfbrbpgw.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mlfkbqud.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cekiwzwk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2cvzlfiit.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2vndnxkxk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lultonnu.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2kkxqkybx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ehqoocbu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nddtmvja.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2zfmeelgi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtwwbzxd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfvfaokh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2hpljbpoq.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2tsjxfhkq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2klzyrfwo.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2hqhbkcme.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2exlajogm.html


<!-- 参考信息 -->