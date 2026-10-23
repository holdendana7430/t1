代发 wailian999

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3tozobfgk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3runquaxv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3fqvrlqbe.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3zuhrrgyy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jssgwcuc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dducolfr.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3hzzxqwwk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfcgmpfr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3axitssam.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3osocsthj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qybhzddi.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jfouhxgz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3jgdzcdpi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lrlnlrbb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mxgtlkdz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eahaxcvg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qjmkvghg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3cvvloonl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dkxxiube.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pkbzyijp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3evaatzhu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oxqrtjne.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tevccven.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3czocyhrn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oaxotemx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bkbupwus.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3jbqmobsd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lriswegy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hekyieel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lvlzjmzb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ekavsklq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnygabuc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ilezthzq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3dhqwxegs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3olvrqeca.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ghpqybtn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ozvzzivf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lqznxfbv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3zecsbnrl.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3krqwczae.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kzoctvrh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3jfvzazgx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3chvfjmjy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3wgrsezpy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ectkidyc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3grpdmvjy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ysakpapp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3xgcbpxfz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3lghyritx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3mlvezfrm.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xlmqviio.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ekzkkjgu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3voktevve.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vqfieeph.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3houhvwcy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3khpoyuqm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3dkmfojmg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3qghxqiqy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kfkbtqsc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3labptgmh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3khfxonjr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3jchnihkx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mzeayjlz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xfvxsduf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ftuvmnni.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vabkyypk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ufrlhisi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3syayjyhf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3dkonzofx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3gagyytte.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bhezbjek.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hiuetpxh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nmotpbsd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zldzznij.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3hmaneeqq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lvyaffmq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ivbzjteq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3rfbrhrtf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tftimesg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qhwarznq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mbzqjcar.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zskocsxc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ebbswrfb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gxrvbliw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zdoggkcr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tppjcstv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3pxupeyaq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bmixztyh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3flveohry.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3eeiqlxah.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nzkwkqfg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ierqpgro.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3savfifwm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ubpswgyo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wohpzsqd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3uiegstrn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3mgoirbxc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikwrfocc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jvhtlxyv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3yxitqeca.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dgjlgita.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uillnnbs.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3iwyqjhcu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3pfmavpmk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3mfhvrynx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ipqkydgl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jxeczxvq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ktuqxaxj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3dzblwfjz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qflnkhmq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3xosudwcr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kiqsxfsf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3addbsdvy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ieaueyok.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jzqfdclk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3coxbespi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zojbaccn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3myqcomkn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3vffztkum.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3annwzmox.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tmmdgmax.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lklzmvwq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3fspsbtnr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pdpfdoft.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pwtoflos.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wejbcjhy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jhffzate.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bgutxmgm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3pirpkhvl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uxtqjfum.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3xzrylsio.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3lpowfybh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3bcfjphwp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3tpbplhat.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ukmojodh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3fmcrhbie.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3pvcevbai.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3lhtnrpke.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3eywkeeom.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3lylomgrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ezyoyyhj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3lyrbwljx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nexvysfl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3zcxlsgfe.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3dubclfrb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3geqdgrlv.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xioqywys.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjaqrzab.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3pewojysg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3rzqwlkfv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3csbzlfiu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3prwimbls.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ybdbbpuv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3vswidczx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jklppwmz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcrdoifh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3knrxvlgn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tufbvrrp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3imxxjsht.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nsoybbrm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxitytkl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ztvbxsfq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bbzzphaf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qxiuifxb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yslbsutg.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3irmoyyrx.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3vcjkqnie.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3pjjpofbc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ksoigjvf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3svujpjro.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3uweccmxy.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yxkeiglw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pjtvhudi.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpazpvnv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwrelmlb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjqvrieq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3efvfgmxo.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3smddxfue.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qblmtdcr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dcujnocj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kmcpqycu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ueuwnsgc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbeaafvr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3meyhlowk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ntcmnucl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3purgpxzu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3adgotwxs.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3odbsbicw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3fenncwcv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3reiyyvyr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3imuelfur.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgvggtpy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bcyoxekp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3npdbdpyd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3gjhwlypx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3cndnfhqj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3qfwzfmsy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3zlfmgqqp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qhxuyswr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qfukcmow.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yjymyxrb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aobciyuy.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3phvvpsvi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3mquetmst.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3eefoqepu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3thnhonli.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3gctyemyn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3rndbektd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3urtpptep.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3kktfqkgy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ilesxott.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3odmsrsza.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3gnkkrapr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3vpiygquo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxoiohmb.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3kehvmbul.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3osjckphi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3urbtyaub.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3tcsnpjzl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbufuwps.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ctrcpcri.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3rngjwwwu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3sihfziub.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3crfswpxu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3diujbrxv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3lwjppjpt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3egnbfonj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fkntyzgs.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yaxthxuc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3qwtlepyg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3pnrprjhx.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bdjbfwrk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3nhjtjyir.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3dvliaetc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3navzkfit.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gvinkqcv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjvvupwd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggxmigtz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yoltmkpt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jmdkssqr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3iprovodh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptbxjrph.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3greuluxh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hnknmrvp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzrpjrvx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mlwurwee.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3njeeuqcv.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3szrnkhzv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3roasxtxh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3iyhhcwuw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ztcflaxz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3rrvivlpe.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3kgschhqg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wyuxjetr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rshmpjmd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pozqwmeg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hxwaatcg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3gedavlmv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3iptrarvf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3fdchvlrn.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3joqtctzm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3axzmlfqb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3adcqfgbl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3oobqukxc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3qrrydwtd.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3antqfvso.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3mfxogsvy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3vompvtmy.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3sdzcbtse.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pqxlacvt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3xbuqzhfy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyzmqfvp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3umganhjz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vokuiguo.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3dtczbgco.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ijuadshd.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3gafrbcxv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bpoqbhds.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3vvsuwnyz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3vbkpxuvc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3xtufmsrg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bznbnkhx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dwfvopjq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ituyyana.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3jidojzhz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3zmjygtvy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ywoofihc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bsoddtwx.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ntpmagsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tujcdule.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3fsseodno.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3cjnfvpkg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zywaiqbj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vopsfzci.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wnnwkvxk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtofvxbj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3kdqondby.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3mgdfyyhd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3gevekqak.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3frbhsgcx.html


<!-- 参考信息 -->