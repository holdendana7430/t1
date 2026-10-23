代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3kxptbfbd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3oarzyrkm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zfdjcyzf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rdqjgibq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3reygctrx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3dxrkfgmm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wkwfpasn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yystftqd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3fxiwdjek.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3efkwtsgu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hjvbeyzi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qutigfmf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3usfjxvwm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3eektykpi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3hwrdxlwb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ispnsrzg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xdsrqgsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bcvviyxv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3vwerngst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbfbttkq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3tghbpngf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ejogtwru.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kguwvdpt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3szckbiwi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mcrybvyr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3brzdusvd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3fvacyjpj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mnedebez.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xszgctgk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xfuntlmg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3fxxyyzvg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3heuafaml.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3feagvdqy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3euiybtoj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yvuavcdi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3evwyniug.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3kupyygaj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3skufhzvt.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3kkwesoyt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fdejsozd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3tmctrxxz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bpfyrzkc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ftdghfuz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3sxangsyh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3vhldbsbm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ifetmxcv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ecqplsst.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3jszdtgse.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rrkhldez.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3xnfhabiz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3uhejunuq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vitbpwzd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3jjfqoarn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3sediuvfe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3kaqzqoxj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3nliehmvz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3sjqzctsm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3jrldphhz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gynxymld.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yjrmoaob.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aazsogwc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3alsggbvm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3nyewkfyz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dwfxfara.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kdclslot.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3fowmmnqj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xwktikkv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cbirnylo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lmhyneaq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nuurkkuf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wzqroirn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3epynpgis.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rojydsvn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lhjyaaqk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3hfauxieo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pkgnzcfr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3jcnitxyu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3oqiiywtk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3chilockx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3oswqxmoa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3twiasapi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3oahaqzio.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3uzzqzeog.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3adqfoxmq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3gnqgzscs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxttvobt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rdiqdzdi.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xjjqehqi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xvizygna.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3nlichxat.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yfyaaaiy.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3bhcirgib.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3jbkbrggj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xbdgfiif.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wxmmfhba.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ysyallbd.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3uylsodrc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3leanlwje.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3qbpngsuz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wiybjlsu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3vrghjftb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xlbjvwrm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fdrwaxly.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mopszbuy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ikrwcqbk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ycasdges.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3wdvqdshm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3guubzqpp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3krcinhhq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3agnqtzdh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3enypdnhi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ikbmumef.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fmyvglxj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lqukjxlx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rkqrayts.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qnsyfzyp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3vzhzghrp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3skvpmxxe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3jzmzvnmy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3kykrmmbi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3whwdsooy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3tczftwtl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3rhvpjlzn.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wzxbybmr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3usrlubqd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3szpqimav.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3lhfdgodt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3lnqdmpke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcegruiv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3djergybi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ogxycxdx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3hhyuuynw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3prvohics.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3pxoonpvb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ecatzbmb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3qftusuho.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eovuzhou.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3yckczqdh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mbhuhfwm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbwbcccs.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3imizjjxi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3cjysrgel.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3hnruvgvg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lsspywwy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3rxkyjpdh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3sbwyjpfp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3puwegwic.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3taikdasv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qfstbyxb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3peooytyv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3aulseeeh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3eyjfxrtk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fvflqdxs.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3foxirsse.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3zhmhvcwd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3uekcffrw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3azstouds.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tilfahsn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3wejolusb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3reyrspqd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zzzebbfn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovwyzyyf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ospinjrx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufbgybtj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nvhkgxgd.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3leqahham.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zdjmdjge.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3adcxwomf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xjofaouk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3okgbmjbq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ywzasiho.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pemvjqob.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fjeznqyi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3uzuancsm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3iaypimku.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3idaekxes.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rwarramd.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ervzdblb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgqsjvth.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3apveepsf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ovwykhfe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyjbrygw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3lmvzjyjt.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ztdhtgej.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3okfbtweo.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3feflbhrl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3urnbgkuz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3wrlskvfw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kqcwzymm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ntvezjgi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tkzdkiti.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3idpiwtrw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3uokrmhvy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ajaftmrj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3qecakjnr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3lqobgfxe.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkwdrkxx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3rmxspwoc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jfthaczz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3cjkbylyz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3naiejbry.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3qzevmitj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3rbllscdg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3qigsxlhx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3rnqnhjjc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3udnqtkrj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3lgjglcxe.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3alahxsns.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3qwmccfzs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3lkxogcxk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ujyccggc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3fvayfgjp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3nrjapsho.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ljjsjjxm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xqqrfiin.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3zroulzpx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qixborfp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3qbragizz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3yzvdfwyr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uvzqqhfg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3tawzulmm.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3hzrcmmhp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3mnqzofoy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kfjjsjzq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgvxdxbe.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufvvdhwi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cjajtlbm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yykjufon.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3nelwlchp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mdbhbgon.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dxaytgqq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jlytooys.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qnsenzco.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ythzdenh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nspeqzem.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hiwxicjs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fulwhwph.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pzdhztcu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3loxungxm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3pebqmyjq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3sytcdjxg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rjpkmqpi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3grtaxlpl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eswzwcdm.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nfzbzogc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3qnefwegu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3qfgiaxtm.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3dgbbasha.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3avcqqvrg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3anlxhyga.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3tvphlejq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3yshfnwih.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3zamalfcf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtsvcjxw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3gvinasbq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3emyapyiq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3akbwuycd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3kxdeiuoj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3xzzcsruq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ubxnshtq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ucaydine.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3dgbaksuv.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3kgvlxklp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3wfqtwzuq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3gmjircgm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3npoqqkki.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3xbwcrvun.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3oglvviim.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3epqtmejk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rpjrlsjk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wqxgsxby.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ncraqffx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3qaoelxca.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3qsmqrsgh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rtmopgej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3binncryr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kjdhfpsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plqkgxqp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3nqmdqmhj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3cmymdura.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqdxwsiz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xvuylexh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgtefjbk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3dxvocogv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3elxvypux.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ayasbgdl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3mwbtmuli.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3fxtsixvh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3tfqzfckq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqteyntj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fysmfjwc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bijdkmyq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ltvpwatx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ygihnsum.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3vhinknkj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3afiphixl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3alkeacwh.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3yxnhrdkc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ilobmwig.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yrajdigv.html


<!-- 参考信息 -->