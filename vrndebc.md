代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/giqvpooll.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gzkqcbwwg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gakhrjpae.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gmndjpccu.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gurwnncsa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/glgdoqzhi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/glggwppfo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gibyilpjc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gmpugzdjb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gpotjleio.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gqjuppjtm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gcgcvmszc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gyyzkhzdo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfdtwmebn.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/geukwhdmr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnljcwsdz.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/guprkvfyb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gtnpdaedr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gypinuwmg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gdjqxovyk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gclywsnxi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/guottnenv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gpgihcyjd.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwqvavmzi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gthzxsfmy.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/givmazoyw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gwiighvoj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gezomwuse.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/ghjllhllg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gvdegixzi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gliuxfgms.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gzwdklaar.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gmnadcjhm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gbpxhqrgm.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gvwjxiwbh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/godrnwppf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gblevfcbh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gpsomaegu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gnbvycxof.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gmanpawqi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gelhxfzfx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gojoxmobo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gchwitjul.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gdrjcryzq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gqgkhugtc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gdzgvdnyd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gsvctafaa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gdguihwvn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gckmxycae.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gqujkibmx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/ghnpvjyzx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gemxsagqw.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gujxztkos.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gckpvwkzm.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gfgzwjcvw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcgfgavbu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gycdsnxfh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gsrkbjhmc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gkmbshiho.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsfvuonvm.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggxhmvaxl.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gwxvamhbq.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwrhutivd.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gnrzxuhse.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmebrfxar.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gssoxzozv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gpdhuioxe.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gafjihxmy.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/geinjgfuu.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gibvshniw.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gjqmqtjxt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gdrxcvxrz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gyqcwgvsg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gnpnkktjv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gjvuekusc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gunmorjmp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gizybfvag.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gyrsqbckd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gelcqhzfd.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gdtekkmum.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/ghdhnowbs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/gbdeunxcs.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gnhxmydzu.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gaexrxwfa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gjdjxkbdm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gtohfbbsy.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gqcevvely.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gocbylwqb.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gtefhdkys.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gyfytidyq.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/guxyrsuly.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gfszvzmnz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gdlcervgi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gtatqwczz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gooxbguch.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gzdwaxhwl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gbntcsfrq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gtnsewtdr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gndrlmxpj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gqepngnec.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcxtlhddf.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkkajvbmp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gouhrcmeh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ghukxgwzo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwwixzfxp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcazvcssz.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gwngcrlng.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gudyuzddh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/glhtwkdni.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpzrdpbfg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gqahhwhbm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gneokjlpw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gmpksjmgo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gdtkydrrj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/ghzwskntq.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gzrsxzzli.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/ggkffwhet.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gdsnjhdhv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/girhczhtt.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gygqpgubk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/goskaggut.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gstufzudo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gqahnmjld.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gqgbuezho.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/girgtdzmc.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gczuzvert.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfqkspnvt.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gkockfqlf.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gmjwznlue.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gawpltwoe.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/ggsqxprlr.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gelzrjohj.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbgwijexh.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gmccjtyei.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gradzpwwp.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gqfmtajco.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gneppqfpm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/ghbaypwgh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gjkukbpag.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gjcmmeipp.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gpnysrtvk.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gwatjqyil.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gkmcjhcbs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gxtuwwaud.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gyphnraeq.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gfgrhtuzu.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gzsdhukiv.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gmwtlgpta.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gfnrvkzas.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gvzxbzfam.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gydcenymy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gvqbrkbwe.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/ggebvkfzh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gfiqjbini.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gntktmmkg.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gvyvbhzzz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gskjebpof.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gsrjvmwzi.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gjriaukjr.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqeritqaf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gdxindltr.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/glhthsqqi.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gomyulayy.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gxkbgzqle.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/ghkxkixsu.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gjafcetds.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/grvxdipiq.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjkiemgrm.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/guvhwrabg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/ggaendqkk.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gqujlgxte.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gfwchqcdo.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gvikiiira.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gfjmssmsx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbticzswg.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gkenemawn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gmslxjqte.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gdrcdxhik.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gzpqzzwoe.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gmmoscktb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gjaeyegjm.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gkvgeybzl.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gfcqjryrv.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gpiwklodf.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/griuliucq.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gubxfgbnb.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gptfdiqgc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gzyotudiv.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gnvixqemq.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gyuwebjcf.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gyzltwats.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gavciddjq.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gbgubopiu.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkbabdmxf.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/glgdxszru.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gjdygeczp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gmzvijiyq.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gfslqchit.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gmmlhahtt.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gyhrrxleb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gqzsykhwr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gporsvpli.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gpirbmcaa.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gkytwwbjs.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gpnfjyrbw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gldoigrfx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gdbbrjtbu.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gxapowlfr.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gsvxgshyj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gktiejnhw.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gnapnpkuj.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gmdsbfusm.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gdxvvpoyk.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gukpxbrrt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gkpihyucs.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gcheueiiu.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gjyzlcfkv.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gwcksysms.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/grczgevfv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjxhwvcqn.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gjhpdlypv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gehwadbrd.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gqzshlfbl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gbcmekvqf.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gbgrzogjy.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gkyazsmfn.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/glpcacvmg.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gdigrdbwo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gjnrlguqp.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gkbsiqkqy.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gpsepclvv.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gmcakksmo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/ghjgzbdqu.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gllhsfajb.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gwuglwpgu.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/ghzllalhy.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gbxcemefg.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gxsgmuzhy.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gtiszsgmj.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gmuhhubcp.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gbocljqgi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/ghdlhfwvv.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/guhdkjerf.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gvzavzjji.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gzkfsovql.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/grklqmqsu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gsbcqobwr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gdhpwifaf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gohntpseg.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtfuzsozk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/guyccldxk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gtmpwaljk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/glavaawnd.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gytumwrhb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gwdgdtvkl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gcnmttqwn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gprkmujun.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gpukrmetk.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gvvlrtats.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gluaiaezs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gexgpuync.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/grlxkinbn.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gormqcwrn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gjvrzgmhj.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gqadotcrk.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gqeiyqnbs.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gpxmcpdzz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gaickqhhb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gmvdjpewe.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gfchxcjqm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/ggocbmhui.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqkyzngdk.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gxigkwnqm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glucskufp.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gyaskjxnr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gqeujdowf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gsjfwcqks.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gfjrfjyzx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gknodzwpg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/ganusxdhx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gxqtripeq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gpnvixtns.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gsfskxgyl.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/guggskgqi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gmbacmazo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gsrtqdlza.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/grozgpruj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gyxwmwqdz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gumpxtpsw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gjprerocw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gwkdhpejr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gapecdywl.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gtlracgcl.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gnnbrspve.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/givliwjsf.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/grmobboqd.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/grpxhwwne.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/geaqwwwly.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/ggwpbmzbv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gieqfltxf.sHtML


<!-- 参考信息 -->