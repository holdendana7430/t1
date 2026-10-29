代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gftmasavt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gbptpfhro.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gonsojpwt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gvihbihxa.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gmkkztymp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/grsyxnhlm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/grhfvqrkd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gjmzhoitc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gwudieeuz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/goravdgvt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gvlameggl.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gxthcuylf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/girtisinf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnglmthth.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gamhzqrhv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsgjqptcp.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gvtkmdmwi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gnywctefd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvjhwtktv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gmlrubtit.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gcbcgbvwg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/giojmireg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gnegsbsip.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjwcgrnyw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gstuarxro.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gmucrzmzm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gpqlxtzjt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/giffvupwu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/ghkcacypw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gvxrkpagm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/ggwqgomme.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gkkhnxnsd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gcwdulses.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gsrxhtdrf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gujxdaogw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gojjctlsx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gnnskxqgh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gytzxizep.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/geeoddxnx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gfkkohffj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gzcjnlyku.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/glzogqlag.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gsgethadz.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gjvvgegqn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/ghepjzqpt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gvqrbshst.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/ggeroymfb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gddjqivtx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gizusbgyh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/giyxiddzc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/grydjlfog.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gqbcrmdlx.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gjytqyktz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gfdflggnr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/graksphov.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjfjupdpj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/goipipjln.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gadysqbdb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gzznjwoxh.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/grlivnpsd.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gayaobmug.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsbhvrecx.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/giteybvdp.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/givalqojd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkrgmskly.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gewoxlbgs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/guapqxjqw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gaeynqedf.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzqmwoucd.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ghngnzbqd.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gpsgoinxx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gdbttwbac.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/ghohzqmwe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gjtgzwkvw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/grxuyrpsj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gvvdqelgc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gaasdvxmp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gtdluuuuv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/ggtyliwdi.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gjfrxyvyn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/ggyhmkyhe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gbkbitadg.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/goreqsljf.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gquyliogq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/goundffjz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gqsuwiryd.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gbldzgocn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gywzcphec.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gxqazniye.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmetluvry.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/giplmkatd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gmjhbgdeg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/geufpaiux.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gkvyzfjlx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/giufmtekq.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmnkgmnsv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gsuxowxqd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/glolfodps.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gybyhevfs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gepzoccsa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gstlbtpuc.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpbputgdb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gttjwbrkq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gbendcydk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/grjzattxs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/grvkwvgoh.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gvvdxcmbk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/glefsabst.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gtyvigagn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gdpwbewtf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gnyjiagzq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/ggbcrbwvw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gjkwxrbbe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/ghhinymjw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gskbaherb.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gwkpywpgo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gpockltab.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gullwoycu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gfmjfznkh.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gmizlitxn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gpowigqde.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gecfxtiya.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gququneiz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gqzfbtdgg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbhzpqkbr.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gnqjrhunp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfoibfkuf.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gmtmfoprq.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gpaagocmb.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gppmsjnsz.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmfnmqsie.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gtukijxbk.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/glpqdeyce.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gyhkhnvoy.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gmrqlkajj.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gvmhdfawi.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gppydlacu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/ggpanwdjp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcqgwolib.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gldawhqii.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gslnybixh.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gikzxjkjb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gfzvgslil.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gtrytecsi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gwuiymbkn.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gsozryjqy.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/glvtbetkd.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gwfdfezih.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gxyyygpdy.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gxcjjseqi.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gfmsdfbjd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gfvixbggm.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gxljavjyc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gupfckhgg.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/grjgknkwb.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gkhitsxua.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gydcvinle.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/ghmhzflfl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gmaxgwbjb.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gzdgtqqlo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gndkkzqha.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gptxzrqyx.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gfqlznozr.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gviwpldkd.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gookkurny.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gqaymgsms.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gequentyx.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gyqdurazr.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gpnosocjk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gxfosmimt.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gnijxuhvk.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gwlbkxrkc.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gcadenrnp.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/guzlgyqnk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqctddfiu.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gvstjbnic.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gepssiahc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/glgzgoxzd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/glizdtmlp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/girxyfkwj.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gsujiaxzf.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gvcnnebxq.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gdigqwqmj.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/ghypmjcsm.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gdfbuczch.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gvvdorqll.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gclqbatww.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/giioiilpc.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/godyjlvxs.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gmwsiwquc.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gwxyyxygi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gkfeswbzv.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/ggamtveqb.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gplltxekx.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gbapezdcq.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gnzitjvpc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/giriwnxzy.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gscmmlwnj.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gwbadldzx.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gezoboglf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gmtpuuhwj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gooxfhszs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gspnzjhnu.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gckurlbqv.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gwvkelffm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/ggxidvhix.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gomrlhard.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gyuhhnhmp.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/guwydwqmi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gvxsxugyt.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/goitmnguh.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gwecaraph.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gnfztfxih.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gapvapsvr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/goobrfaej.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gzqybinot.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gyivloapr.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gfrnlmvcg.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gtukzufcc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gcyzdcrlj.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gepdbzdbz.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gmbtuaqsq.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gijouxqzp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gvffzrwms.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gzkmqwvfc.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gsbwdxznh.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gpqreouxc.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gzytmfprk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/goznatpum.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gnnmdasvh.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/ghegqareh.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gvymgparh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gkgxksdvj.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gxwdhjxzl.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gtawwczjn.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gonssuehi.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gdehgpolo.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gbqewjwfa.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gghvplytt.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gtxcvtiop.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/glrlecpud.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gvtxxyhrk.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gjxutaove.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gixuofyee.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gqwjrgwkr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gtpucisvk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gmoyargaz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gtlqckhon.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/grqcuvnqt.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gxvmspmyl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gdhsojaui.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gkkqkjgiz.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/glwfoffxo.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gijmhuqkg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/grwdtcmrj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gnbessebq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gfzavgwdo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gltnkdkgo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/ghqubsrwa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gprcozqsr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gwenhnwnr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gwrcbtnpv.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gfaapjmno.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gusukduta.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gdljobkmo.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gdjrrwamj.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gvyeyoepu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/ghlmvojwd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/griiestyw.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gqvyjiufu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gzrjepcmr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glhiumsds.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/grfksxkjq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glluhjpok.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gukzowlmc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gtpdcutos.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gxfzwfcvh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gunzhkbzb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gudlqhvql.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gwjlnionx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gwmsvzoqv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gjftvfnhg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gnpjqoxcu.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gsuxkfcbx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gzkxzxysk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/glenrknqw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gmnqnzwxh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/ginrsqves.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gazcdmkwl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gqrsxwiyk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gozrqjnmi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gihjkucvn.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gryxpcybb.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gsjkjelmn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gqhgcszqq.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gjdsewvkb.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gomohmdni.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gljsgukyo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gaebeyice.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gqqwvifrm.sHtML


<!-- 参考信息 -->