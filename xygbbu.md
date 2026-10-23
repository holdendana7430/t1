代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rhsjnygh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3nfrafmnd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3uyytbxud.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zokizovv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jvevclwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fnwrzjqf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3mfipyxdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhdvhfon.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3gwvxivis.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3dfhloqvu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yujozxww.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3fxtpmdpf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pfcvroxx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nseunzgp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3djqsrkwi.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3psejstnq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3loxoybhy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3jwndahcf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3zpftkgss.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3gqdntogz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qyunulzb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qemgctku.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3smmanynt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3qnkkwczz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3pbsybcpm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3gecxwaoj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3esytgdwa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3vyesriie.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3litkconm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3eowqyygx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3sqxixivg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3uxzzjmfm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3cdsejstg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lsngahlj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bctfjrjx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3kuzcwioy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lxnxxdbm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3rfblrzyv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kzbmekug.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3bmlrujfs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3grijmvuk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3sblemzeq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3nywdgjro.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wazktrop.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qauvzkde.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ufwntzzx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yvxwezgh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yzcitzhn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zufafpep.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pnhykpkw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3sbieyrcb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hwalffyu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sbmufway.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3zstxugwb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vgcajfxq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xvrfphfq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bmkppmym.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ogswgnnv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fmxxbvcv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3quwlanpj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iellwyjf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aocrhken.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3sffhaaad.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xwwpllpb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lndwirzt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xsnzytac.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gxvehzfk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3rtasshwq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3hdaeigtn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jeydatpp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3mhkwlvqs.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ayuznenc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3lboevhgs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixayoanr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nlbejeur.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3cgcxxhhm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ygklokfy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qbzmvgkc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3fxycqcyw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3wbjfowcd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3lqixtlnz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3keisnpvl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3atwaoyov.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3oqhwmjrg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3itwvspqk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hytowhxz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3feilqwjl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gqhgfezn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3mvvhbhdt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3baeqtezf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bhbhhali.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ksvnsoqq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3epgsrqgx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pchqcqpo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3waczeypd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pvexzepp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qljwzrzd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dpemhjfk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ymmghfog.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tohadkde.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wxtdobec.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3idpdfpyq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wdglpqim.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ehtvfdzv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3liaxztlh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sxpcysrw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ptfjlmxs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3lhtugjoo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3pipreolr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3veqnftyz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ednafdis.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3chcazopg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3acdclayw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ssnixcdq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3zszqxdic.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3wbgtnxsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xapcvamu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3eaqmasmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqhmzzyy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3vpfmewbv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3dkmdrozv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkenqrzo.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3eykmiuay.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3qfxojmey.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ethkkalu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3wietfsmz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ndkobjjt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jmdhtgjo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3uijvncmw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3iqnlsxuq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3mtfppsue.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcfmzqcy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3iktsqidz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qprsdvej.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3pqdkvuer.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mxrycibm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhvvlsrh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3cyksmmfz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3flbyrjhp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3udjvkoix.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mrzfxyqe.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qeoudbob.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3tqcvzjgf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3smqmvxvm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lvljzctn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3bmzovmda.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3honkmxos.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3anqnqhzz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpxejqeg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3snebuvmp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oblizlgh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3csmwnsdk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xstglbmp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uredzmlf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hstlptou.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3mvmjfeyu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3cmxkaacr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wytabcsl.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ykltmstc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mbydavia.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wvgpzlmu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ojutgbur.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wtyitsqo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztalwwcj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3unjjngnz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3fuwaatiz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eygvvscn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oopvsyas.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mvrrhpun.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cmctipgm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3xftippca.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3qessjbqy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ybddkjjj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3nkihomex.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bphykgek.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3inpdqqgx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tknqtopr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zmxjdfxr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qyivzwpk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3sdupftso.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3filoqfha.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3meieqhpl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3fowkffli.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3exuigvgc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3mlrjqddo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3zpzfdtys.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3bzpyxodz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zktadbry.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3pmrksrzz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3hxlysdhm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xefcvebr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3bptromto.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3dlicioiy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3vrjcebcn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qmkjfrcs.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3buwjptrk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdofxtyq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3kggvmefv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3kijqhyah.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgtupgsr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3orjuhsgu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3cmsugxfc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xgvvaymx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jjinemim.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ucviipde.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3olysgadc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zvnfogak.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tmqevoku.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3znenjdid.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3aakashtr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3sogcydgu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ptzagumn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yufzgpxd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaglutlm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3oftwhodq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jmitczem.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3iqccisno.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3hxvpjukt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3bxsgzndj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zxalxgrs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rytrjjsl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ywembtum.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcayxzac.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqycoqcn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3erwbonde.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3weisjwdi.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ucdighkr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3bsfwdqls.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3xksrdqnr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tkrzvszr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fiswlcaa.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hqpqsabo.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rbsucmiu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3qvaysyvv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ekdoxpvl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3plumlyro.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3duslltuf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3sdfvwzsz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3syfnmiur.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ekpsdwuz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mrnwlnqv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ryiintqj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3qmdoglkc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3oukonmsq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3wlezpudy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3encjpfmf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mukcwxxb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3govcguuu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3gdnerinp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ffbhdqlw.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3jglttaec.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3zwxwfnxh.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3zijakkbv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ejlucscm.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3bycmwehc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3unyavzql.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3pqqycimy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vydqcolk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bqoeuxor.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3mrcnnmka.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3cdfkmtdu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3gdwiakpu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3akfkyhlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ognccsbj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3avklqqwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uauhkbaj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3omoeiuoc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3tdlgzdpk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3npvbxyri.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqanxvbo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dybludem.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3nsgpswnx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3borwrxuw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3aafxonth.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3oqagaeor.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3jrowqwgz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3gcixolcj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uinkjzsc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3crnusrwr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fmfkosbt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qqnnyplv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3sczwnqjh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ioookexm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnyfohlx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3juptbkig.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3qjqpovxr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3smrkkqxp.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3eptqradq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kqjynelr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uxcrgqip.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3bhdjtwqm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3wfvsuloy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vsedacxc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3yflaffba.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3aoetmwbh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3broacqav.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3akobwpsc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ayyeckya.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ulydrioe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3esewnflo.html


<!-- 参考信息 -->