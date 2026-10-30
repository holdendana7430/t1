代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/guswivtrw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gnyxwvqzb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/ghuuzbtqk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gukrenujn.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gmalgthwl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gvourbwgp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gafbaazck.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gtcbojwkp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gkcebapxe.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gmpiiygni.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gcuyfvyux.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gmmzogmjw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/giehomagy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzufwrjdl.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gmqqvvlvl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpblbgasl.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gpwitexrj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gfmqiaumv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/glfycintm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gzmwnzvsq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/godbymsfx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gkpkvcbmk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/geveirizf.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzmihjvzq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/grodxgeoj.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gxcvddlsq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gbzejczyk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/ghcqcpbtf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gdpofxsbs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gezqmtiwo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gqqdmctcr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/grolrdodn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/godqtfrxu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gapgbqtnb.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gmckrsdwd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gdkbclaoa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gqaxyijbr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gabuldicx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gzydevruu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gxfkvdixw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gnmftaivk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gceuvjdas.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gzpqyvbcs.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gkzitmhkg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gzzwlgwub.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gvbikyfjh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gziaihxgt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/ghavoxoek.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gczlqympk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/goirybjvp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gciafqqfb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gdkrbscdz.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gazbwteip.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gznetpcew.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gscvwrfay.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwjpyajzj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdehihlcl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/geppiwmte.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gwuieiueo.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/glcpubsgi.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxilfvdws.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gbipvpgag.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcmlucnzk.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/goskyoule.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwvvpvhvx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjtipomtk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gaogzimkv.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gkwaatjds.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gyfjmsmyv.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gnyozzqdl.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gzjitfwea.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/glftiacvm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gghsotofi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/glhqnvnmi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gdeunzlxk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gpjfnfkel.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gkjmrhvsm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gjfbfvadm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gcnpgprlv.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gfhfiqsaz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gnufytobk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gwneystxz.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gqcwnaosr.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gvzhygjri.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gnzblcfag.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gxokdttvq.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gfdsdeqvw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gadtkoaes.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gzolahggo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnfiyvigr.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/glvehmhou.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/glkhojjpe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/goliwdvag.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gjurrwoei.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gycwecctj.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbdtdqesh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gqkytxhsc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gtjulxjui.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwqylwdhh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/glvqgyqci.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glailxejb.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghmyplllj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gdbdhivcu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gblshzyfx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmvvdkktz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ghhdmxgnk.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gwwjckieo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gaozffkih.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gxzgayivh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gwhslhztx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gvltcizpa.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gspsezxiz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/ghlnkyhku.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gtojxbppo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/grpgodskl.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/grjnonkbv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/glbrumvhm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gunpnsppp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gvirdrgux.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gvabggrtv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gkttqbbwb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gubbqnnuj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gvqregraz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/grfcptshp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkalruwea.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gtbdvghbn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guzhudifj.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gqhqwdlmt.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/glgotjodn.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsxjgyykl.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gduxyehyq.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gkoyugjmq.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gwcxldotx.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gxbyarsdz.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gqwstxzjt.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gfvrcyzwx.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/goqaviiyf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gtftmchcy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gldghgnpm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gbhytdwbn.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gviaiavnq.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gdduxwolq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gfkgugfbw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gvqmgfkzk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gubhuxwml.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/ggvarkrpc.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gjugromrw.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gvyhnuvbt.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gohxfpvhn.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gmznadqvd.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gqnynymyk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gdziexefg.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/ggmiocpcy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gysvbbcxy.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gnhjuwrud.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gmjfpsmpq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gzgmemdil.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/ggmvmuote.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gjpycckej.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gjprfdvxq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gbfelymly.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/grxkqzksl.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gwntthlub.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gqhrfpigd.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gjrqrtlme.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gubnlnhda.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gnlbfzxwd.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gdneimuks.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gidwmgykh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gxrheicfd.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gxpmhikgw.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gfgxifokp.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/ggbjgztwk.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/giijgpbka.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/givakgdwx.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gdkkevcjh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gqcwojdyx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gbjmulokc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/ggckiompu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbwqrwpri.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gwdhjxupr.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gjlcacamf.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gufeoffuc.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/giimqreiq.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gmoqxfcte.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/grtauflrv.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gnogfkjho.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gypsuystj.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gjjwucrtg.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/ggypupgzc.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/ggkfzafsu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/glpvalvke.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gondlbcge.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gmhemvsbd.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gavylwvux.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gqtedfwpx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/ghchutbfm.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gruoojboh.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gdttmswah.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gsvwroatg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gqlshpelh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gcwajglbx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gvsmaixpf.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gcdhpwxiw.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gzjzidncm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/goktuspvp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gtxdgiqoa.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gcyqyjfiy.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gqhgjljab.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gicdhcwss.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/ghdfqiwcc.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/grjbaggcj.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gghoascwy.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gidvwtpwj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gudeagkyc.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gkfvaadoo.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gvwrggmeo.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gbvqkdohz.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gjrrdtuxe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gqisminuz.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcsnmfapk.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/ggjixmstg.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gcctihjkk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gaidqgpsf.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gmmmgzltv.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gsrhklkfu.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/geiivzejy.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/ggdndyfkh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gltjpbdmb.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gkfeytarf.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gvngigeyg.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gezgqmsvy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gcqomyzik.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gxdmjteey.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/giwzyludw.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gutsttxip.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gmrtbaqbc.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gyyshstjo.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/girimjrjj.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gsbswzvqk.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gtmoqpzsh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gdfwdaukm.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gvzqgzuru.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gdpkyupiy.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gqbejrmfj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gglxsbetc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gedfusfqo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/glprccwjw.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gdtrfchfb.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmkdzbhxq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/glfpmrmwj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gffziubsv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gzfoxrglh.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gzbluifrt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gvriisktc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gdfebhtvt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gegdhojjm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gnxbsbyrn.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gfjmokiqi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/guscnugod.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/glnysnoqe.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gryxnrnzm.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gxdlrvgyn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gjnijlrpj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gagalbjzl.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gaiquuurk.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gkojsgbnv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/grqftthpb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gdhtjkfwt.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/godlgxxnu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gcebuvgae.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbydrafqj.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gvquotmag.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqwemhegq.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gykqaiejg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gzwjnqhsr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/ggfyycwjq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gojqenglv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gpudxesfk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtuajatvy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gzrnwczlo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gappphrqv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gpftpnjbv.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gynslycou.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gjxclqqjh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gakdyovbg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gjkwyvycb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gnzifcleo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gtdzqxonb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/gfeftrojx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gqyvfyrep.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/grqyxoaex.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gfirftnnx.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gmwpbeevp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gxlybbaio.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gcxfggwnk.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gkfhchfge.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gfcspgwpy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gjaywwtcp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/guhxhucqi.sHtML


<!-- 参考信息 -->