代发 wailian999

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3dgnmdbpp.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3bxiqeodo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcnlmvbi.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3thkxlrwt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3dzchxgfx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3sjtudkap.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3efflwwtp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3idwgjsdu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vovruocc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3eqtmtdan.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wmwxfnjg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iwfmyomi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3gdkpcjvg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3nopuupbq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wvcgceuw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ugeeohpd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nejtnpvy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3swbrfhlk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3oatzvduw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cnhnaicu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xjupnlzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3onuspcxj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3nsbrjqmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzmyjuwn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3jxxjbwdl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3nzacmmpb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dphuaurw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3qkxsiklv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bxplxilv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vxqhzzqd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3odcyfmqy.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fqzakvpx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gebkwuhy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3cwrjwavi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3dofcezwl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3njjtynwt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3olovixni.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3sqtclkgq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wklybkoy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3tzfkclxb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ymxyorjn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3yhoighkz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3knnygbwx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uqiguwbt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gszqbyhk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vsufpyrt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kxbsujph.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xvrxwlkv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3huncjkay.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qcmciewr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zecpxspb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3kbyjxzth.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hrjangpu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3mcqtjurx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xlvqevsh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nmyempma.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3stfdceaj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kdsaqsey.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kgvzurtt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3pbfjtama.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ghmgtoxt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3vavupkmi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ebmwtndn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fmskbfzy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hmhokjbv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mrepyypq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3dvznfacr.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3prspvuqq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3brrskqsy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ytvdkkhh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rinpytku.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nfchoemj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pkicucls.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ascvmuwz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xlaqsojo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oryrmrpe.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iprxztsd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wperqwwx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3tgcawbby.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uzlegoxd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ihaxeocj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zzhyffda.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3krvqfzar.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3gxvplzeu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3jhfqcnkq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3tewuatli.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3nqqnrqqv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3gfzddpwr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3whprzgvy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3jospdoyv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cmcopqfl.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xzsadefv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dfhagqux.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3refoeuem.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3nusalnoq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3epvcqwuz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3pbzarpbi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gvwmfihc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kznlcazn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xhbdcoaz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lkgrlelp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zmhtohmu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3cjkyrdtu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wytdeotv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3zrcevzji.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3sooctihb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rvnfzbqv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gtvafiff.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wohtijkk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3famcmaux.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3bbmspkkv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jvwvdrmu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3shmszxkm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jdlpntcx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3zokpbspe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qzgmuiel.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ouvnkwde.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hlzqhnng.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fidwvkls.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qcilysxz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3hkfpylwg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3twumkvsv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3zrrmzgnr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ezbavvnl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3lobfqpmu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3xtusnxcv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3zrkhrnis.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3puhhnhdm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3zbtxvsoa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ilohxcps.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vnepjjsn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3fcckkusu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqcohouj.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3urkuxfgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzdhxpxr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3kdgsakon.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3urodxhpm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qufzujau.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rustivyl.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbkxtrqx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3dqdiasrm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3xppffktx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3wkjryegd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tdsjswcs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ywhsrjou.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3gjajbyaq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3duklhfrn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nppdkxck.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3scjllrlo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uwaagovv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vmrlmrxn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bsbvanwg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3izppvmhw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3qcpdomdy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ybppumys.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oiqgjiqa.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zarnxtwt.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ypdrxgcz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3iqjhwlou.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3jbmrmsir.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lxmgilsl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3yjzmgwkh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3uosxvujv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lpvusjsp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wntohyyo.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xcrsnzfl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rdydjwbv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3edfjeapi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3feotttpy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vsvvdhwg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3eeftqhnc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3mxylwlyt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3grzdidaa.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rlvsynbw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fkkejwtd.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3viwovftd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wghnyyfc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qlqkxcyo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3pgyfwoqv.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uuyjvetd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3nbjkrvad.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3emtpbnjv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvdnwmbo.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qmocnnmy.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wydexdyg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sskehqhs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3eebbjbuq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3pkyrzztt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3xlvasjzk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3uddstsbk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3iirywgys.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3avtmeobh.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fkrgjtkk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3buvnzglw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lmihyoog.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3qipxtrir.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3nezvicbl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3njwpaldt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3gkycifhf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3jbwzjtup.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3yeqeimtc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jijextom.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3vaxoasns.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncgtjthm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3clwjcesv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3zsmjezrb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnlgjuxm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3vvsqvavw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3zvpnevwp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3zlckyfri.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3htljqthc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3putuzmuo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ostjbxkk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3dxhndmwf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3aphwrqhn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3naubhwds.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3nccuflxl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3vsdeziof.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fjubqabz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3tbgwlqqk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xrnkvgtg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3cfromcfg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3qeshncgz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wyngpypx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ikuhunfr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3nlopfhmh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3nezuusrd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3trrfwahw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrbpcbpg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nxlmspsz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymtpzcwe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kctvxjqg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3wlnufwcu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgqhrhhb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aphhnhtq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3brhtcfgl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkduaorf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqwlygyj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ieydkste.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjplcwip.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3igixdzuk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hfpkcsdb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zsudekyf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3zixxkfxm.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ppsypbvw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wnjvbnrq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wpbwedkm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3atxtbowb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nbdcnvjw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3fpezluia.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3zmduorxq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3qfrjiuou.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3fxktjiij.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3hsrzuiiq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3rlprifvv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ixdnekvy.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3gjmgckqm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3idcfaicp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3qoqxiiso.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ehyfmgnp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3dxhdcidv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3wafdlgiw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3yqulhxbt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3kxjnakuw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ghmxsdqw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kiyusbml.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3jekwiylq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wmdoqsbc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3olrvqxat.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ngjaibru.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3bzzpgvdp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3vmbqkblj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3zjrkbrpo.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ynntusbs.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3odajtwab.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3hmaxsscu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3zlmdnoeg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3kwlvyhex.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xvvbdvzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3adntagmo.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yjwyphvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obnxotga.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3igtalkxp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3coksqxpl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3akvvicpr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqtewxsf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3slapjqzc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3udvuovqr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3umdvnxny.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3acdxoxon.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3oyqstycz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3gllvxqee.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3bbqnxzia.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3karvukmr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwkitcem.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zwhhrlqa.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dyfnkmme.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3wkbxncws.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3fbgliffh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oepbpgzc.html


<!-- 参考信息 -->