代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ihvhkzsa.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qkpjgvjf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3czjncolq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mzwrxvhx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rbcpnudv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dyhknfuu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ieqqhdwh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3vvgrkhtc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xjkshwpr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3vhfsqumb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mykvotbp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3samcckyv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3vzlueock.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3hgyznadk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3rzfuktpk.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ektafyed.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3dshykomi.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3dlfatjfj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhraispk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ufkutsuy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3fvkyilon.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dueuplqw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kshzwjci.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tymmebkm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lrmnvejl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ovivmhwq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3reiputzz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fowgqznd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3szbvgrzg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ionwojjx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yvhvsact.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ltnlnpcc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3addaesii.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vwsrqzkd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ztrfsuqt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xzfxwnow.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ogiizoal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkzwmqvh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3peudnham.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wapdqosv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ewiunqve.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3bwnwvfju.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xtsfliie.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3oiwjoevx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nzwhwjhb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zccucpwm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3oobqtnpx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gdzkxagq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xoiisvlz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3xujeefga.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3tmlavsti.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3hqkfuhwd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgrppwib.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3grqkcatl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3flkenbwl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ihoaejjp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3pculnmlw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3hkzlwxmr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3quistfkw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3uukfslby.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jholsykc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yiqqgmww.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zzckgdox.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3fvpanccd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3tblqotyq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3abwudxjj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vrxgfoun.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3jasblief.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3odvggbsw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3dlkoksss.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wedakirv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3duexkytx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3qsarqkki.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3clbhvacl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3aiklvlbw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3uybaegbp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3voszicva.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3hpcqrnin.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3owpiwcfl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ybjmnuca.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ucwsnwaq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xtxtpbud.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wmrmvrhz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3agxexkwt.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3veqsadsq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3btmbtydf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dxfehqso.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3izypqazt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jacsguxp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iytnyysr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ycclkxec.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mdqwdsqn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xgavehea.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3femcrdyh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3epjojlhj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3fqjutzqz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ybiiwbxx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cemcmghu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qgncpxwq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3iwmrqxko.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3lgyaesxi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qsghener.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ejbggins.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3xpnnjrnt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vnggwwlc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3psrsskxm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3yoknwbsp.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3dpwycxky.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3imdrsnuy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3dmwiuxhh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3bksgmkxg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kbopsjtc.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3tqaujlzw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3axpeubsm.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fhicngmk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lhtqpxny.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3geskruwl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nenydvfq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3xlnfhbwf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mzrvmyqk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xeajdvcd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3aeuyfmzi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tsktrntc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yridmgso.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uebqzsxb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kjgghbhe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3myztajcc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xmnfpcnu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ozqjawov.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mkyomfqq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ahfvgpix.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dhciiafg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3optepbvj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cqnctohu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sgfuxhgn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yvzyjvur.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3wauonpqg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lzfrppsi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3cfucmcir.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3eblbofut.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3zhciurtv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xmswvghs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qxiywsmb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3fsmcchur.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3womeftex.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ehvzipbz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3izthztuh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3rqitduhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etzwhtkx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3axsnpxvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irvkvany.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3pxowcvxq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ljehjcbo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3srsyoifu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3clmylzgr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtnzmeoz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3hcoekhlu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ofgzicwj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jkdimbeu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ttwwgsex.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hekbbouy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3mthsxija.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqcdsyvx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dpxcuamx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iiqrhzta.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3clybhzlx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3xzxmxbps.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gqmseoju.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zlhqufsm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3kbbttxym.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ktlrjgkz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kfryqwes.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3iueiaxmg.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3asmnudyn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3jbbojelg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3pntmsqom.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jhqvrmbh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3yljfjqim.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3fziajovd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mdbrovcw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgumkgdg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ypfirrwu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kqsnabwn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcsmbezk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ltxsmpwn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rmhdctwz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wpmzlvki.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3qgnjvpgn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3tqjaxzcn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxjkjbwt.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3txicnvnd.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pbvdvnix.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qgbzusnc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3uarkycic.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gxqmubgu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3tixrdupn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ipuobqxl.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3recyjyvp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hmjdhjjn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyjwgthk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehxphnza.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3poounuot.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3exzgmftm.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jyjgeyqz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3doldsbgc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3lthxtthh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ckjcdmlx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qqvgsjnn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vhbfczca.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qekxmjuo.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fpxmfjur.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3shmwwjvi.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3oozdpbza.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3esyzmvnd.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3rxjryyjv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3bqmprgsw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3khfloxbo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ukccloer.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcyhcufu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfchigpt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3wnmlfuyb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3wqycsnsi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ndjtkmto.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3pzsuuduv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ebdkmvro.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyygypqv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ltsqoqia.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3odeoonhb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3mzqacgmq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3lyyfrilj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3rsxyqidh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3agnqelnb.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3zxmrowrc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3hukvvohj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vfffyszm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3lmdsotqw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xyayjhhm.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3dsftdryt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3rapgvfkx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ukhecjoc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ypniwaak.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3awhntwxf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3bqjsmlkg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ateuxjki.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dymsgbsu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqoefrws.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aqhjnyjo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zycaxjup.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3bkblpqds.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3kldxqspz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eexrnysa.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tghdphwt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nrzelufr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3apxwoixr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nucnskau.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtzwrdtw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vsrxkwzg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mxbhaadi.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gvbxextc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3unmuuyka.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3rkmqemod.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hisbgfmq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qnvwulzz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3htadgzyi.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lleflbkc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3lzgilvlw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3phpnhjqg.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3nhafyvqt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3sysaglrt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3vokmefza.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3tspmbkid.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3hqqcppga.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3xlpybphv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmlxoctb.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3uanrtzyt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ttrehuvf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3vwznejcg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3eslclzbp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3zuxewwom.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3owdvmitg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xrjlmrjr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zvjbagdc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3zxafnhpf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3keybluqc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bvphimiw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jquiggbs.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3grbczxsc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3lwopvgbv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3iuczissq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kaxkhpma.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rylibyfk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3clohbnkf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ohvshqqv.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3mdvlqmpz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hmvacfns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixjnhyll.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3vkxyuozt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wcghvcjo.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3zxlyefkn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3torgrzza.html


<!-- 参考信息 -->