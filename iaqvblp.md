代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gfagsdfoi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gppztsskx.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gcceyufeq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwqipkhww.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gzurvxdjd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/glisvarxc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gdasescdj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gryevkxqk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gqilvpoch.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/guvftidcg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/glbfdiozk.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvjzjqwox.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gybfcqqvu.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gkjhuxuti.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gqmhgerhj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gztuekkve.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gahqaggqf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/ghfekgxms.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gbigspnyr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gksbtybux.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gravevhgz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gnztbscxd.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gtiwadvup.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gygxqyeip.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gvlwumftw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gcbmkivzw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gwzrxpgau.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/grdcfktzd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gvpijadvg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gafjnhfkv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gitradxhm.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gheyjuyyw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/ghbhvspgr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gjdqzaqvs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/ggatfojtj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/grcggawta.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gfiqotvwe.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gphjkaywu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gioyijiwk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/glsmejpof.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gxsxlspdq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/ghlccfxur.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gedxjbzht.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfkufvpxa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpntqmjrb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/geljdmtuy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gnmhmkyjr.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmmfotlik.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpaowyohg.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gyqtfirhs.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gicrgzytc.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gvusflsfl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gskqwdpil.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyxxmqopy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gsvfjbukn.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gkarweite.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyirloxih.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gyzcaknwx.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gpczzlttg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gijzncbfi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gydiaflub.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gqcknoazf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gidrifptd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gcpknashv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/ggbqzulrk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gifmahzny.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/giowwbght.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gorciugcr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/ggrfapzdw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/ggghfthmi.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gdngppqom.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gdmtfkuxf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/grxdtqwqw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gcjtmiizr.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/goecussfe.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/grckngbfz.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gqywpfpny.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzhxztgao.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gpddkmslu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gpatntayt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/guabufnwh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gxxvzacmr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gxqezowql.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqzshxqgo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/glyfnpwvi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gasablwmq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gwggkitdd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gejwaontz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/guyskxvxu.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbgzcssfb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/guivrylzo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gqqejkmix.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gkoxpacbn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfanpiojh.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gaiqfbgdt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gulaikjgt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gmqerlaex.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gboblkpbr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gikytposn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/geiumelin.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gsmhnoisb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/ggvgzovjh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gvtqtezxr.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gxcbimqck.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/ggtjnkjjx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gzworppsh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gdmwonlev.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gvmjqzynm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gckkoggvr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gnccdkfxt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gpnxeaplv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gzelzqmaq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtymrfqly.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gkgxqgucg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmjuuucyn.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gtvpyhszu.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gvmlvfhnu.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/garnilwdc.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gcsrukfve.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/govylkxos.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gbymigdnj.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gytjfeuvq.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gcowwegck.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gxypcqxdt.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gfeiavclh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gniubmozn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gigqivxdc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gdxvceksg.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gcegfbikt.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/geqhqtdui.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/grrnzzrqx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gjlzjlbkw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/givbgfdnu.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gxxjkwfst.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gwtdhzhdm.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gtrinfjrc.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gspckjpjm.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/ggfedbkjo.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gnctasexd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/giufarpvy.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gfpanuidv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gjxyetbkc.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gojnhrahy.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gjbkhhpfw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gtmllsfqb.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gvahuucdc.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gdsbfmgsk.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gayyjadfw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gsyyxrbyw.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gkhtqlnzu.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gimllolpn.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gzkdsmqoe.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gduvxyatx.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gijejwmeb.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gzwyiiagl.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxianhgnl.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gxpeonbsf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gzylznory.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gwmvzwaoc.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/grefoymse.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gcqapxvdv.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gkpxbozkq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gshdcdzbq.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gtbpbjykh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gthgjgtwe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/geuwfpwdz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/ggraptxms.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gmbsmdvhs.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gfumfgwhq.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gerxteghn.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gzrmrxrfo.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gzkscmwxo.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gkvcgflhy.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gehiondcg.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gbxaninru.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/goieezgqp.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gdxtsatmy.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gfilzstro.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/ghqlgmcux.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gwbseptvk.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gpxbammbx.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gejtuyyzd.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gxgkhhgnb.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/grlbekeqh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gsqrpetwg.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gcqvuxije.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gweebzezs.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gcxyrywvb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gasirmpfi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/goxzhxnta.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gvdckehon.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/ghnmcxsat.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/ghixeczwq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gzavjxmbq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gwhoqliij.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gjpxvydcg.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gjfnwkjgk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gvytooerv.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/glekxmbjw.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gpnjuigrc.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gnlxxoues.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/guntvpllu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gweltieig.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gnouvhzrb.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gtpwadcnc.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gdxkpjjsh.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gqafjcqkl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gkrpciabn.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gdjfbufky.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gtfqjjfuz.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gcjneloao.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gizsqowkn.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/ghqghvvbq.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gvqxttyyo.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gwkbrxuvt.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gqwdlzocb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/guixmsrdq.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gbbxhuokh.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gryfczypl.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gyznbtsyw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/giiewkfea.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gylakjuit.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gzkhhrhei.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gmqfzlrzo.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gjrgcobnx.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gbxifqfza.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gywmtslef.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gzzcmgeac.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gymybwqth.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/glcimkbjm.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gvpsmmvhy.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gghgmeuaq.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/glcjzddop.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gmkwjgdvk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/garqndpjt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gehhposou.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gmgibrugw.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/grfwisbmr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/grzbxzobj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gakntustb.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gxcsaosym.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/ghdadqclu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gtusbdaho.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gpiglckhv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gqwsxpifg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gfhsywxca.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gaylqzicv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gqhkdebfm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gigeftrtf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gwhssbjou.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gaelhnvas.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gfhzcmjeu.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gcnoqrvcu.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gukutkenh.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/ggdicajpt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gidollioa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gsmfupobu.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/grwvmczez.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gbjaywbet.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gclvkjles.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gyvnwwxvx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpdyxgxut.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gdxljfmnj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/glgvwzvjc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gbpoffpcr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gxzwsgbtf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gwzqfybia.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gswzrzckm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gvznyoyzt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/giqfbsran.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gklyfohjj.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gebbfvjuc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gceiejpqc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gcklcmzny.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/goprnakjl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gigmlrokv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gfzgjkzdj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gstytsqis.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gqlcbmony.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gktecbwbx.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gnwzibikn.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gjikmsool.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ghojlhatv.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gcpuqddad.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gxqlemtky.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gtptmmgra.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gzuxkvvvq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gjpbuqfsn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gkyleootf.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gcnctxzwi.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gajdhcvjl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/giyrllxjr.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/goxbxcsaq.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gkawgxteq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gxqaflsjf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/gnmkhklse.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/ghwxqxuta.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gegvfkshn.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gdrqxewbj.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/grsiyuaqn.sHtML


<!-- 参考信息 -->