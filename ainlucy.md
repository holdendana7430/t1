代发 wailian999

[F01] 读取整个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrhjmsqk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpsotdhi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gfisqynbv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbyomixy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fanxiaobao.xyz/Article/details/giyojzdle.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gieklwrob.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fanxiaobao.xyz/Article/details/gvubjihyp.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrurvljl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqrbfnat.sHtML

[F02] 逐行读取文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxboiosam.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbbtaizm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycjieksp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gzvqpmqqf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgmtvcpz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fanxiaobao.xyz/Article/details/genfjqauh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpbdavmu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fanxiaobao.xyz/Article/details/gsjkyfkad.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fanxiaobao.xyz/Article/details/gxdeihghn.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fanxiaobao.xyz/Article/details/guowfnixg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzenbxgio.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gdpojultt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fanxiaobao.xyz/Article/details/gweiyfxpx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhvrxkuc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjpxzrue.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsfrdqrw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fanxiaobao.xyz/Article/details/gypxqucvh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gwonttzhb.sHtML

[F04] 追加写入文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grsiiexfd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gseilpukz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fanxiaobao.xyz/Article/details/ghdoamakc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/ghltfkqiy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfrlfiov.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawmizsls.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduaneslg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fanxiaobao.xyz/Article/details/ggteqsxff.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwuuqtid.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/grapkejji.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrumajhp.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmqlfukl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gitsvrnwa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gdbeagasu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gminklsso.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fanxiaobao.xyz/Article/details/gmfkxecsc.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyqzlpvm.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnqaqdlm.sHtML

[F06] 删除文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggfscsgwe.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gngjqoclp.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/giapntlmf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnundkotm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpmemuln.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gaoaxwlxh.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhvwvbvy.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gsoagfilm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaeltgif.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fanxiaobao.xyz/Article/details/gijsfostk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfwmpest.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvpluzqn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fanxiaobao.xyz/Article/details/gpceizxia.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlcddeth.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkndplkcb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsklzlrfz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fanxiaobao.xyz/Article/details/gttnvfqoq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvuokjuu.sHtML

[F08] 遍历目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gszqxvcsc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fanxiaobao.xyz/Article/details/grzvmiyhy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkvjcumzl.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gmjaomxmn.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacahlaee.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fanxiaobao.xyz/Article/details/gordfjnuk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfnjndec.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxedgxtkp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gadcupmsb.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxnnkser.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvalvhby.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkaeobzn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpythrwz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fanxiaobao.xyz/Article/details/gytvynqyu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gpwzwjthd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fanxiaobao.xyz/Article/details/gwkjmmfgb.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gwubrjpja.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gkesibajo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fanxiaobao.xyz/Article/details/gmqhgujot.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkbgokuz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/goopeotup.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/geaoksaib.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gjyiochao.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfuvuldk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoslbwyn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/glpiealrl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/glbtfcraw.sHtML

[F11] 复制与移动文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxgpxsnoa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/golwpulqo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gkvxpfsxw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/glzjdyjut.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjgtibsh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groiycohv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fanxiaobao.xyz/Article/details/gptvdnoja.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtluvhak.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxwluztc.sHtML

[F12] CSV 读写
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiclztya.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fanxiaobao.xyz/Article/details/ghrnrayst.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakpvfktr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fanxiaobao.xyz/Article/details/glnhthugb.sHtML

TS:   // 同上
来源：http://baike.fanxiaobao.xyz/Article/details/gebrowtzv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwtqdoym.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fanxiaobao.xyz/Article/details/gukiiljbb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fanxiaobao.xyz/Article/details/gmtdavzbm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fanxiaobao.xyz/Article/details/geccpoahq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpxahrlbf.sHtML

G. 面向对象
来源：http://blog.fanxiaobao.xyz/Article/details/gsvftbnuc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxylxllj.sHtML

[G01] 定义类
来源：http://wap.fanxiaobao.xyz/Article/details/glakkstnw.sHtML

Py:   class User: pass
来源：http://mobile.fanxiaobao.xyz/Article/details/gjutffmit.sHtML

PHP:  class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gqxnhmgzp.sHtML

JS:   class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtwpwngcq.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grtomzgqk.sHtML

Java: class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlxncxjj.sHtML

Go:   type User struct { Name string }
来源：http://wap.fanxiaobao.xyz/Article/details/gospzmnir.sHtML

Ruby: class User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gypyvvlyq.sHtML

C#:   class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjnregja.sHtML

[G02] 构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gprgmutga.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuwubdgl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgowwzrj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwlueefg.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gvvcoqxpa.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpwzejqqn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fanxiaobao.xyz/Article/details/gzpbrbxlp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fanxiaobao.xyz/Article/details/grgsluarw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gscstnnuq.sHtML

[G03] 实例属性
来源：http://3g.fanxiaobao.xyz/Article/details/gztunwfxd.sHtML

Py:   self.name = "x"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnturwhm.sHtML

PHP:  public string $name = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/glgemnojj.sHtML

JS:   this.name = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gcglhtjyn.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdmsvygb.sHtML

Java: private String name;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjfnbwkg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxvjdtbm.sHtML

Ruby: @name = "x"
来源：http://wap.fanxiaobao.xyz/Article/details/gyxgeqshl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykptptiz.sHtML

[G04] 定义方法
来源：http://blog.fanxiaobao.xyz/Article/details/gsbvsqpto.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fanxiaobao.xyz/Article/details/gdbngamcj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gaghdtfbh.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gminamfxs.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeoygktt.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyapxxan.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtaswabsm.sHtML

Ruby: def greet; @name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gzxdkhuql.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlkpealj.sHtML

[G05] 继承
来源：http://baike.fanxiaobao.xyz/Article/details/gplxunskj.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnostvlc.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjofqino.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaerwibe.sHtML

TS:   class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gptfkhvmg.sHtML

Java: class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gcohrqims.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fanxiaobao.xyz/Article/details/gpifcqntz.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzqmsdsc.sHtML

C#:   class Admin : User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gecrtkwsw.sHtML

[G06] 重写方法
来源：http://blog.fanxiaobao.xyz/Article/details/gmgpgedrx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutnqciee.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdamfxscf.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gehaohkkb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwhotexzp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjddnqtrf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fanxiaobao.xyz/Article/details/gurmkends.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fanxiaobao.xyz/Article/details/gwfzinxom.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fanxiaobao.xyz/Article/details/grxqnguof.sHtML

[G07] 调用父类方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/guupzymok.sHtML

Py:   super().greet()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkayeuqy.sHtML

PHP:  parent::greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoicxnbt.sHtML

JS:   super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyjtukti.sHtML

TS:   super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsxjnirg.sHtML

Java: super.greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gjblcdqin.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fanxiaobao.xyz/Article/details/gzroyzqfe.sHtML

Ruby: super
来源：http://3g.fanxiaobao.xyz/Article/details/gffrzijxg.sHtML

C#:   base.Greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/giqgaeora.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffoqhxad.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnmqbgvh.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgwjsoqb.sHtML

JS:   static f() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gampwxuqm.sHtML

TS:   static f(): void {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhbxegaa.sHtML

Java: static void f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtaphplqi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fanxiaobao.xyz/Article/details/goubsqnzk.sHtML

Ruby: def self.f; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gezlaoyuu.sHtML

C#:   public static void F() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gtledkywm.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqyiymvh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fanxiaobao.xyz/Article/details/glkrdhvhm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkewblbkh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fanxiaobao.xyz/Article/details/ghtrrozwd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcandkuxj.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaibwivif.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fanxiaobao.xyz/Article/details/gsszptdnd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fanxiaobao.xyz/Article/details/grrklyegb.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gdosmrhzx.sHtML

[G10] 访问控制
来源：http://blog.fanxiaobao.xyz/Article/details/gpgxgdfho.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fanxiaobao.xyz/Article/details/grnqkpaxa.sHtML

PHP:  public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbxrtjmd.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fanxiaobao.xyz/Article/details/gojeotwwi.sHtML

TS:   public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/gouxygtzm.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fanxiaobao.xyz/Article/details/glzizkxwo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fanxiaobao.xyz/Article/details/gtjlpbksq.sHtML

Ruby: public / protected / private
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmyxnaiz.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fanxiaobao.xyz/Article/details/gujsdtzfz.sHtML

[G11] getter / setter
来源：http://read.share.fanxiaobao.xyz/Article/details/gaabitomp.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fanxiaobao.xyz/Article/details/gietxprqf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fanxiaobao.xyz/Article/details/galhxzfsg.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxpnafyc.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpngswsmd.sHtML

Java: public String getName() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvofcqhge.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyonzzbj.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmhtcbln.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbuvjznr.sHtML

[G12] 对象转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gezgbrctw.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsoxxoxu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmcvpxvmy.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpewxkzmm.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghnuldayc.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvddcmeu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gnoglkbbv.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwihndcef.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcuznpgc.sHtML

[G13] 判断对象类型
来源：http://baike.fanxiaobao.xyz/Article/details/gyrtzcvrj.sHtML

Py:   isinstance(u, User)
来源：http://3g.fanxiaobao.xyz/Article/details/gmjpnwypu.sHtML

PHP:  $u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gjnfjzahm.sHtML

JS:   u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/gwxwbapib.sHtML

TS:   u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/glflxkytc.sHtML

Java: u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/gczcrtihr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fanxiaobao.xyz/Article/details/glwuvkiis.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fanxiaobao.xyz/Article/details/gvtdupitt.sHtML

C#:   u is User
来源：http://baike.fanxiaobao.xyz/Article/details/guyzgvutv.sHtML

[G14] 数据类 / record
来源：http://blog.fanxiaobao.xyz/Article/details/guugciiqa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxskyxzgg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgxkeafj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdaktgjv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcxhhsmd.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnrcslvs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxobqfiih.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fanxiaobao.xyz/Article/details/gvvpatyie.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fanxiaobao.xyz/Article/details/gbmjomrxh.sHtML

[G15] 枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxqqovqk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gpcggqdth.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyyckewv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fanxiaobao.xyz/Article/details/gdidotkfz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvzwbvuh.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fanxiaobao.xyz/Article/details/gilckrfym.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxesrncw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fanxiaobao.xyz/Article/details/gdbnlfgod.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/geondvryr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyckfnisu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fanxiaobao.xyz/Article/details/grlpeoije.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fanxiaobao.xyz/Article/details/gufcmgjpf.sHtML

JS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/govcbqsad.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdgrvofr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfzspqdr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fanxiaobao.xyz/Article/details/gsswrhhrd.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmmrkhsk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fanxiaobao.xyz/Article/details/gjdrxdgkj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrsdkswk.sHtML

H. 异常与错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrqeqlqq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqgrvdnyj.sHtML

[H01] try / catch 基础
来源：http://read.share.fanxiaobao.xyz/Article/details/gphfxujak.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjpqaise.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gfckfbyyo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/ggwxccpvw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzrinull.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fanxiaobao.xyz/Article/details/gejrdevhu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzejcqwz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fanxiaobao.xyz/Article/details/gnqzurcts.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfonkwrqn.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fanxiaobao.xyz/Article/details/goenzjpaz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowvjnykz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gejnflyhi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfalhwuq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjhnxcvq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggegnoyeh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fanxiaobao.xyz/Article/details/gesfcvpbg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhenveni.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/genttazyc.sHtML

[H03] 主动抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpjvhayz.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fanxiaobao.xyz/Article/details/gngnydmwv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmagmhnz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gucvwpmgz.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjkjjfov.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiewyrxf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fanxiaobao.xyz/Article/details/gchswyyer.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuhsxpse.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/grpekobfa.sHtML

[H04] 自定义异常类型
来源：http://3g.fanxiaobao.xyz/Article/details/gckoaiwgs.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fanxiaobao.xyz/Article/details/gygerlsrq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fanxiaobao.xyz/Article/details/gutrdgoil.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfdgvkzs.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmbfmaxz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fanxiaobao.xyz/Article/details/grpykalwn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fanxiaobao.xyz/Article/details/gactznddw.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fanxiaobao.xyz/Article/details/gfgtjvjqn.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fanxiaobao.xyz/Article/details/gzqgnsfyi.sHtML

[H05] 捕获特定类型
来源：http://baike.fanxiaobao.xyz/Article/details/gnivbtfrz.sHtML

Py:   except ValueError as e:
来源：http://baike.fanxiaobao.xyz/Article/details/gvbbkimxt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gifhvvxqy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gvqvhrlmf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuosyybf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gavvrgaav.sHtML


<!-- 参考信息 -->