代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gmhyirpru.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gavoinlem.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gyfjuzudo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gvhtvsuqg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gzezclrjj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gegceemhk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gzbkwzqdt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gpsujaaqd.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gewbhznir.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gomtprxvo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gmnxmeatd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/ghcoxbxtv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/guwfpebrj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gblfvfuqv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/ghytmcivp.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gzjkitcha.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gujparcsv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnretpfmi.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gqdnbbejb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnhfzgfgs.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gvgcrpwlq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gfrgpneoz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gandxitua.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gmenupgmw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/ghmjxxwji.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gialojqra.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gkgoizmlj.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/getwealrk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/ghisxmyqh.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gspwrndsy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/ghlxbhqqq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gkwatwopt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gviccbsji.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gnefclrek.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gfqyvvlvu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/grnkpovon.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gjphwbald.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/grfaqfgez.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gisldqvle.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gitslhfhn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gjytxqmjw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gywvfmxdh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gucouctoa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/ghrcozumr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/geiegtsyd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gzkqfusnx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gsqrzmnzh.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/guivyibpj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gpnkouoct.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gdqbfnjpz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gxvmanful.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gjhqocrqq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gsfbwmlzh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gwqavnxsf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gvlidumqt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gtxxcxlzl.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/grxnlcram.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gefizzzof.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gticsikqp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxlrfhokx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gzatzllke.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/grqqirxst.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gxbfbxywi.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjqkcnolq.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtjijuxol.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/grvzbnrhw.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnulpgjvr.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/guoadeeky.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqzrecvvt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghlecucxm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gyvcebcdd.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gaetvxlfb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjlfqorwx.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gxmfvtwvc.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gwxnxotwg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gfydvwnnj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gloaoeitw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gbsifntfe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gjtfrxssf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gdxqzocme.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gxfkinsbl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/grjknnpdd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/ghnlqukcu.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gydvycfqz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gwkxpcprb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gqzgkhrzr.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gfpjtztie.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gbrenrbll.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gwhytvqgu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/geeqljcls.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gsiqfhyhs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gcoqceqjr.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gvvilhaac.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfowxmckl.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gkcefsegh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gpsxmrinq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gqlvdxswg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/giwjquxgw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gkpmevpzq.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqzncsoqf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gstyfuvhw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gkcxubhls.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmfojopsq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gqdvuwmaj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/grnwqiyrm.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gowbxswlh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gktufjtgs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtylcqwew.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbiharnod.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/glfjfhdef.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/guzulhmes.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/glktdsmsx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gsfpliavn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gxnkzdpqg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/guutowfky.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gtflceffe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gtkpkcvhz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gqlegwqqv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gjuissxrs.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gljsahsdw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gkrcfqlvw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gxspareab.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gjbgckhta.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gvbfvhfrz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gnrwonbol.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gnraskdxh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gdttkuqyn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gmpaqjcrs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmmgbredm.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/glrxpgqkd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grjunqgib.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gsmqfueum.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/grbzjphbx.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/ggkhlekcr.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/ggrgzudpl.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gwarhntww.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/glbmusolo.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gftvavsrb.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/godeityod.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gjkxixzax.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gkxmnrufl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gfvyizuql.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gokuwdrqr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gcygjhbwk.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gzyndvqon.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gtbxwincb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/ghyzxdnjc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gxqkjoyro.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gbvlmrrur.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gvapysyei.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gsoffapza.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gutigezkk.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gbjmeslxv.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gvfdwsluo.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gycknedkj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/ggzneygiz.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gpfriofhn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/goytubnyy.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gxddncdsw.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gusgmwfbp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gfgedrivc.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gmpkabrzn.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gninzvmcw.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gygtcadrw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gxmdbpndn.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gyxhkmhbm.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/ggwcqiyfc.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gmqffxusf.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/giwjvarzs.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gtfrpyzse.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gsbmnhdmw.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gnzzwvgci.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gzbgyhvti.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/ggbcswrdb.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gccygwwop.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gxvyeohbu.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gwoublbhr.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/givonjwth.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gcuzhefid.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gpnmivdbn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gfjqrlill.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gtnxqmfpo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gcsccfkhk.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gsrkhvmqv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gutbarinq.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/glmatkjyx.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/grpkjhygf.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/ghrrklguo.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gpkhkciak.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gnxykltod.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/guiuagxfh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gkiojjnzo.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gusziyeyx.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gzwrshxhy.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gkevgpeou.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/glursuktf.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gguxxhcgc.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gpmzxrmln.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gsrtymowp.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gryjzsksg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gnwfbvxan.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gjfhupuws.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gtlwudcro.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gyapxvqhe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gaozgaldg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gvlfrlhyr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gojqpiyih.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gztidtrgy.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/grzyjfhvi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gbtgcluvy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gesciawul.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/glalxnjmn.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gumnztayz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gcbvqhcit.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gpdnjzlgw.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gagegoknb.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gebmvxgig.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gbdipamsq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gkpuaznop.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/ggmyrkbjq.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/guoujrabl.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gydsxlsvs.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gvkiyzbvc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/giyoueaim.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/grbqaxnrq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gufnxzzxm.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/ginfbrixp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gyauwlthy.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gckooyjgj.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/ggeuyocth.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gakeveajz.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gmecruepp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/glndvajyv.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gccrwwvlf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gogtlmzre.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/glazjdpyb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/glmnujqzd.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gexwmovkg.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/girbeadxj.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gwjzjohsy.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gywkwgylh.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/grhqnrtex.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gilfpcbhh.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/geychetej.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/garfctxsm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gaomsehby.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gzewhmtyk.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/guipnxgnd.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gcshkansf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gwmkvpfgk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gscgefqps.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gwpvqxdor.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/giekskhmq.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gnnzrvpah.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gjzjgrcaw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gqsqrujvl.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gxrxrraaf.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gkfrvvtco.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gyywgmiep.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/grralagho.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gwzxmbyak.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gxgpdpeol.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gomkjurpy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gkrjcwvbk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/ggxeodrig.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gnvqrpkpn.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/grtjdwbup.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gxfxtznnq.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gwexgbwin.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/goehguepm.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gksnqdwtz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gehtsulcy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gjqvwawho.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/grzdxdinp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/grbunuook.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/goiljpffz.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/guyzwgucy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqqpyfzpd.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gbvyokyzj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/glbdsixar.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpjhbybar.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/glqhzfmne.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gjxoqwkgi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gucsiybtl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gkycdmdvr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gzrjzexmc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gicqthxjh.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/grcfvzjsc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gzabvddth.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/ghzlwibmr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/guonitphn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ghmfjpupv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gwgiimfdd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gwtadxasp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gesfwtany.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gsjwlejti.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gfvvsxzlo.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gzafdyvzm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gmfnnbthc.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gcftlzdny.sHtML


<!-- 参考信息 -->