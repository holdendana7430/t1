代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jvhtxffc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2azsbziya.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2npshcaew.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ihoeilug.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vpiunywc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2mqadgsgo.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2nblhqwhg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jxcisaeh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bglsfmzg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xxnutxmc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2elqkyvjr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2efjofizf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2pbtjkvqz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2zcpkymir.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2etahasie.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ctzedcmt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2mxwgvvvs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2xukkpqnu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2sklcmkiu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wupnogny.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzohwweh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2bhopxmwy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2nvjieitj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2lfbbjbzx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2vecrfcqw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mmsnvocc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nqhpbcsq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2feoofaek.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2devxhwlb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zrxuesip.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pefsyspr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wkqcpjsq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2vslizbob.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2qezrlnfr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yfzaaiof.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ulphular.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2usdxhyyw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kgryoqyq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2zqlqnwbe.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2twjvtmvt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2kttorwst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzxusodp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2qebnorhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2npumjhia.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pprhesjb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2wwuqeigx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pszsmqnr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2gsgwxkyu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ukcuysol.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tqenrnxk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2hdrskehr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tfwrnxmj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2brrtjmtf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2yciyzusv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2eyyfcdsr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuchbiyl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2iixcjtfc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xecxhmuj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qvmmidls.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ghfllwvh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2oofnrkmn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ncrlodwn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2nqfhqphr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pwnplbhm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wbdruirh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2skcictrl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ydksnlxp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2qlgwwjpu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2oidwbvlp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yzlnwkkg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mhhlwots.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2hdmlsebn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lvbndaol.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2wvfgklkk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dziosdnm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2tysbzbfu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jekgfjrb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zuthhjtt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2bwqptulm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2prrfjxpg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jsbyzrup.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ckoazueh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qjddcbry.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2humdupqj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dzfozshj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cnyyminr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ykfhxhka.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bsfrtrqx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rkapharm.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ofgnanop.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fasjjsej.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tkkebzfn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2isbohsbx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mkxcfehg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rnuumesu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ssomzspq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oifycdvf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uwnnroyk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2tpjvrozh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wxxxykew.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ukyxtacr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cdgcsthi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mxzctfmh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2kjjhnxck.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2jmdzcdar.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2vjhhgtbl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2kzgtmwmv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2gwdeuulw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2iuvuhfuk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2bbohocxy.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jckqbaye.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lvpzvjxh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jeddzysr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nsldryvo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tgvaemxv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vizhrdsx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jrnhikdw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kmcpicis.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eksplyye.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mnfqkkqs.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2cwbspejb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ctaojhxk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2uablrjpa.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yqcqsfma.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gillwoqg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2eqmxysqh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wkgnruae.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2inqkejzq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rxoqetgo.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2annnbyct.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2vohsobjo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2auabplqp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2emqbyhwg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rujnxgxf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2bherqpfn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2txjogymo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cqsvhtfn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tuwyadsh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ebtfefyg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2glxhqdgi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2edzrzmwr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2msomrvdh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ejigvymq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2rxtkivbi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ggvnhgpu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2iqjktmzh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2twoaggrk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dwmsygvz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2hflipuwo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2uxtxdsto.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2xmwjalve.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ahkcgahb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2viijtria.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2fvxrsyqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtokeakm.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2isvkdwyv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2drsoaskn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2awakhcbd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2thvouisq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2jyzkzlzw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcvxcllq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2icwbgytx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2wtzpwttu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bqhvlrcn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kfwdjhny.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2xukpqpsd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2syussbkx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2scyetphx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xthrfiem.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cefseenu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2umhpuiym.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ugbvsloh.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2exisbdtm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2gzmypdcw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qolcsnvv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lgulotih.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ubvnjpgy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2okgrtxin.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2wtizytsr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2adzcibyd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2isnhrxrs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2rsnkxdgx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vhwcjcmv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rqxzdlhe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eftuztoa.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2srufsdhk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzrcqgwz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2udcqlinl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sovimdey.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vyfbnkni.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gwrtrvzp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2fnxwefkt.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2cgmasxyi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iaxnnfqf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2etnlkukm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fqeozmnu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vfztskuz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2fhatfazi.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jjvcsddg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ibdemilw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jrafsvqy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2pwfhusuq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ztnxtxfy.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2korjphek.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgdcjwjp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yegvnlcl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2uieavbxz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zikxpixw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ydryegsd.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jiuuvlwi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ecskxkmk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2srzsoerc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2aobmcdrq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ctfcqycr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2naldsvns.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ziowdshg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2vsdginio.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ppgspeci.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2bjycxnze.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2nbrpkzby.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2fnozdkdr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2crffspbn.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2vposwvqt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvbzceub.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hwpsjcae.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2gmtcdmru.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxpwmgts.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2nsqjaege.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2eqjjrtqe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2vszqvvmi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2jakontyb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2tunmhbge.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwmmnlrd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xgsqdtor.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ilhwbvlb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2avfarjoa.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2esbdbtht.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2xpwkhtjc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wxuuilci.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2toeljqmr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2guehpsfi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2lnsopyxg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pfpninto.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kohhdhop.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2wrwweeqx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2xofqvxti.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2vmvlxwdq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvhfhtri.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tmubbygs.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzerqeit.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lznibvyz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xvoqsken.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2xjvznrwh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2oyzddwbs.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fdiwmdvz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2forvaqwp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nubpjfiz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pgbtqhpq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpkyqecg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fpsuwhlh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qleqbizf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nqqdwboh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lrmkyyqg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2tvootxec.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2qtdvtskn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zpglbats.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2admbvgqi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gqzcjepw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gdsrbuan.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2uzrwumyj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ieuuertx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2nzrmzieu.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2nrwzycaj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2yfiwjdji.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2pcceyvgr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2bshzfbwi.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2mnfwkxho.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2pzzbcxny.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2apdbquyr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2tlhbjypo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2aosheeqz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2sejysbmi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2brghxzto.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lntcakbl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2fusxszni.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ukpzjpzk.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ftiamyvp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2slducakf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2cjdqjowk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rrubsena.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2bmvkaxoa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2kglvorus.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2rexktenu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yvmfeiev.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2efnlgrnp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2sghvjewk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2zdqnejvb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2cwigovlt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xgromtig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rcarmnnc.html


<!-- 参考信息 -->