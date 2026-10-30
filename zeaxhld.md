代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gknllhmmn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gixkvfyqq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhvdveoi.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gohvdkxxh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gutuuiuxx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqmlefqc.sHtML

F. 文件与目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrbprfjt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsirqzjzy.sHtML

[F01] 读取整个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsufmjhby.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fanxiaobao.xyz/Article/details/gzlvbdaaz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjsziwxl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonhmlbns.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/gwrkpqhyl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gmpdcpfnb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrfqogrn.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyhpdfcj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gyfkrefxg.sHtML

[F02] 逐行读取文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzouyucy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexskhpgb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gblzhekzt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/grkicsdji.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fanxiaobao.xyz/Article/details/ghjyzigoz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fanxiaobao.xyz/Article/details/glddphzqi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fanxiaobao.xyz/Article/details/gmlwxppum.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftpvchut.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqvmysta.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fanxiaobao.xyz/Article/details/ghsowirms.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fanxiaobao.xyz/Article/details/gmjfvntov.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gerykayhg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphsgfacv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/gyfwyblqm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fanxiaobao.xyz/Article/details/gouduhpoy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtacxogba.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fanxiaobao.xyz/Article/details/geacxcxld.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjegzmpaj.sHtML

[F04] 追加写入文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfiuejhy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzymzxzbq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fanxiaobao.xyz/Article/details/gqyyhtzkf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/grmizayad.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/givzyutht.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuvpgfyn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gnjhgccod.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gslizwxel.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fanxiaobao.xyz/Article/details/gioruelvx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotwgonma.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohirtafw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geohhkbru.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbzdzejb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqayauuwr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gmzyaqjwc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxphelec.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtsiapuk.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gcokmqcvx.sHtML

[F06] 删除文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqzvligwd.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcivobtn.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqokjhjc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gzqxhnzvt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzhazujv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/goktuefwz.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzerfmdgn.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gsvwdgigd.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gaghtjocw.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fanxiaobao.xyz/Article/details/glflntgng.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyrnacmv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gtmbwhgob.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fanxiaobao.xyz/Article/details/gcbwvyiox.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fanxiaobao.xyz/Article/details/golqwztfn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxpoutzy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvuybffj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbddoqbo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fanxiaobao.xyz/Article/details/gewndeaiz.sHtML

[F08] 遍历目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gucpofabh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgtmpapg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzlhuwvw.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gfuoejbgn.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggslepdaz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fanxiaobao.xyz/Article/details/gioixdblz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndldfkde.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/ghcdegikl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuzwpxnu.sHtML

[F09] 获取文件大小
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcilbxot.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtbfnunm.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqxgvfgr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpliqhwv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgacpwsj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gsgwfypdo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganlyijpw.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsmbftnl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdhrjfws.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fanxiaobao.xyz/Article/details/gqditzlwn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gyzqgukfc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gwjypsmdt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfnrpcll.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gjetnymxw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fanxiaobao.xyz/Article/details/grajdyfia.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtccbhnqx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grazkduvt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gdgrtzalj.sHtML

[F11] 复制与移动文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmaefpklo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/glihdknxn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzngvwik.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/goltlogsm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gclirjxzr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqnskveo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fanxiaobao.xyz/Article/details/gztsfdlgf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gagfkicvx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gizikcxro.sHtML

[F12] CSV 读写
来源：http://m.share.fanxiaobao.xyz/Article/details/grgoshgcl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fanxiaobao.xyz/Article/details/gyyiecxlx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtbhhmnq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxbocavj.sHtML

TS:   // 同上
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqvrvaid.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlfxiomq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gubefpmhb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagqevehf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fanxiaobao.xyz/Article/details/gujnuggmj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjolcrlsl.sHtML

G. 面向对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoxphfiv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/guwlsbbbt.sHtML

[G01] 定义类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucqgbwzz.sHtML

Py:   class User: pass
来源：http://wap.fanxiaobao.xyz/Article/details/ghhuskaxn.sHtML

PHP:  class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gzekxeaiv.sHtML

JS:   class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gpidqgeig.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcsustec.sHtML

Java: class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvxvmavoc.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqbdzhag.sHtML

Ruby: class User; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gljnxtfik.sHtML

C#:   class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybccmlie.sHtML

[G02] 构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxishtlgl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fanxiaobao.xyz/Article/details/gziuqkhzb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmlisreb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbgsdyoy.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtunfilnx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsacghqee.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fanxiaobao.xyz/Article/details/gvylesnov.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fanxiaobao.xyz/Article/details/goxlnrumg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggklvxnsq.sHtML

[G03] 实例属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshkyexzs.sHtML

Py:   self.name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/grxmshwod.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhpwatld.sHtML

JS:   this.name = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoeyngbs.sHtML

TS:   name: string = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/geimmxhfi.sHtML

Java: private String name;
来源：http://baike.fanxiaobao.xyz/Article/details/gucxzflmr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhxkjcgd.sHtML

Ruby: @name = "x"
来源：http://mobile.fanxiaobao.xyz/Article/details/gacpeiysf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgkultwn.sHtML

[G04] 定义方法
来源：http://m.share.fanxiaobao.xyz/Article/details/galztnlzf.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fanxiaobao.xyz/Article/details/geogbbdvj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gndaqswrk.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjwscxtkd.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guadnwmur.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycevoukk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gzaxegdgf.sHtML

Ruby: def greet; @name; end
来源：http://baike.fanxiaobao.xyz/Article/details/gkklgmfpt.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbzlkbju.sHtML

[G05] 继承
来源：http://blog.fanxiaobao.xyz/Article/details/gmioukdam.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fanxiaobao.xyz/Article/details/gawvgahom.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybzyvvsv.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gghfxsoxg.sHtML

TS:   class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gvmiulazq.sHtML

Java: class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gpsakomex.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjasptvl.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gevjzigbx.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzzhvkmp.sHtML

[G06] 重写方法
来源：http://read.share.fanxiaobao.xyz/Article/details/gcybayzwx.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsaiihxt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmknfvhyk.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gibadawjj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbnmfpxb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllplnfts.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaxkpcgp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedqwlohb.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqtdpcnf.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdugkpeeb.sHtML

Py:   super().greet()
来源：http://www.share.fanxiaobao.xyz/Article/details/gupgpftcr.sHtML

PHP:  parent::greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbpkqany.sHtML

JS:   super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gmiqfxurx.sHtML

TS:   super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gobiopohv.sHtML

Java: super.greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwozfeuy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fanxiaobao.xyz/Article/details/gdudgyxwt.sHtML

Ruby: super
来源：http://www.share.fanxiaobao.xyz/Article/details/goedtoudm.sHtML

C#:   base.Greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxioyzgu.sHtML

[G08] 静态方法与属性
来源：http://blog.fanxiaobao.xyz/Article/details/gjjyiavyv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fanxiaobao.xyz/Article/details/gcscfauqe.sHtML

PHP:  public static function f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gthdzburp.sHtML

JS:   static f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkovfuqz.sHtML

TS:   static f(): void {}
来源：http://3g.fanxiaobao.xyz/Article/details/ghqjpiuru.sHtML

Java: static void f() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjgtklky.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjlkfnkh.sHtML

Ruby: def self.f; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbxukulo.sHtML

C#:   public static void F() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gwklidxny.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fanxiaobao.xyz/Article/details/ggdjlccnk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fanxiaobao.xyz/Article/details/gnfbsjzgc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqxhyfqhl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fanxiaobao.xyz/Article/details/gycdmsvjq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glkmlbfhc.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gosifbkxq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknyzevsw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fanxiaobao.xyz/Article/details/gzckvdpkw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuoyecoh.sHtML

[G10] 访问控制
来源：http://wap.fanxiaobao.xyz/Article/details/gcvhzgqop.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxojsivqa.sHtML

PHP:  public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gcjtzucla.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsejqruvy.sHtML

TS:   public / protected / private
来源：http://read.share.fanxiaobao.xyz/Article/details/gvefidyjb.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fanxiaobao.xyz/Article/details/gewndbfzr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fanxiaobao.xyz/Article/details/gqbgykjgp.sHtML

Ruby: public / protected / private
来源：http://baike.fanxiaobao.xyz/Article/details/gudajmbdc.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fanxiaobao.xyz/Article/details/gexkrjucn.sHtML

[G11] getter / setter
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajtyfwtf.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fanxiaobao.xyz/Article/details/goiubklfg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnqzzjyyj.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfkckhwj.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmbjujnnk.sHtML

Java: public String getName() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvherzhnx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gcygyqxil.sHtML

Ruby: attr_accessor :name
来源：http://wap.fanxiaobao.xyz/Article/details/gagsztixr.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guqgrfyim.sHtML

[G12] 对象转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gslcckasp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtvkbvve.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbfbmwps.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gthajfmyk.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbhlcvhra.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwuoozmf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdekucdm.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbvavbjq.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gasrwpbhx.sHtML

[G13] 判断对象类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhtsasut.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwkjgqea.sHtML

PHP:  $u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/grobfplkt.sHtML

JS:   u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gegmjcwii.sHtML

TS:   u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvwtvjtt.sHtML

Java: u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gafsblhqa.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fanxiaobao.xyz/Article/details/gfldahmce.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fanxiaobao.xyz/Article/details/gkweshjej.sHtML

C#:   u is User
来源：http://mobile.fanxiaobao.xyz/Article/details/gutgitspk.sHtML

[G14] 数据类 / record
来源：http://blog.fanxiaobao.xyz/Article/details/gkipcblvn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fanxiaobao.xyz/Article/details/gcphhwajm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fanxiaobao.xyz/Article/details/gasijpebn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzsjprkw.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fanxiaobao.xyz/Article/details/glmodeeev.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbujiljak.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrkwdxxn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fanxiaobao.xyz/Article/details/gqslhulon.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fanxiaobao.xyz/Article/details/ggqvjmxpg.sHtML

[G15] 枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjunhjwm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gsyrgfpyf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grqunjyeb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fanxiaobao.xyz/Article/details/gaynpcikq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/geibvldbq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfogemrah.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fanxiaobao.xyz/Article/details/gxneuufqm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fanxiaobao.xyz/Article/details/giizaeqpl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guguvtesg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiutpmzu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggihvnrsg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzzchqev.sHtML

JS:   Object.entries(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gsajrztzj.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/goxaajcwi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxvpctdk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gxboqsxrk.sHtML

Ruby: obj.instance_variables
来源：http://baike.fanxiaobao.xyz/Article/details/gkffiymlh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/gceizlzqy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxiataydb.sHtML

H. 异常与错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gaoopehqd.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmudjjfx.sHtML

[H01] try / catch 基础
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqhzrwmr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpautsdbs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxnrmcqb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuqtvhgy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gkjderini.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaaqidak.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fanxiaobao.xyz/Article/details/gqpkrdgbi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmmxiyne.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gktfugfam.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gvabwhdyy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggimhjrk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gmfkifnci.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsusamrya.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/goazhmmia.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdegoyafq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fanxiaobao.xyz/Article/details/gmolnxcvl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxlcqwvd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhsinpwq.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdypittl.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfitmmouf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gzpvxdvyn.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gijvjrgwy.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwekzjehm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gejtkxqas.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fanxiaobao.xyz/Article/details/gksntvujz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fanxiaobao.xyz/Article/details/grtbzozbt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjujrbyk.sHtML

[H04] 自定义异常类型
来源：http://3g.fanxiaobao.xyz/Article/details/gwvwabbel.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fanxiaobao.xyz/Article/details/ghevxsxij.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fanxiaobao.xyz/Article/details/gzrobilnl.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fanxiaobao.xyz/Article/details/gdglkqewa.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtelqzhgf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysrqhnbc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fanxiaobao.xyz/Article/details/gjigbhrmh.sHtML


<!-- 参考信息 -->