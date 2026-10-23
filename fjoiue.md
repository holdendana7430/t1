代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vrpwrytf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zfrzchvh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kllwbrlk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3lvrqicra.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3cesqllwu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3xnaxzjvf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ybkzrndm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kkvcyfmk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3uyqkwgon.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zndcuyfg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3fyskjfba.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3cuqkkntw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3euwubcyk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3nneveysa.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3vwvmptsd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3eeuyxubi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3kztgcnuz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3oshtvmwc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukwhwckc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3scnbbflz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rwolewfj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3omatepyc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxiqtwda.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3tbczgewn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3yzeiymkn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uvuxahsp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3txfnpdms.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3unhyrmyn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pnelbnmn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3bpjoefba.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3glpdtvjw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pijvzbmk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3szlkzzks.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ctzanckm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qolhucga.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nzkbcojv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qrsmutfj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rrxhkekw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3zhjgktjj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kcpqszer.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xhfiolni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htjubahp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3bwmxggqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ywhwafvg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ngzkcubo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3uqkzxyfg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kfltvmhk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3llmdwjcv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3busnbodd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rosnvbqe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ojsnruky.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zdixfjtq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aengkrcw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3hpmkxfho.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3bpzicqer.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wffvgzna.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3skeqwlez.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwinrues.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fqujvqwi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3haommfpr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ubyavjxu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3euqzcxfn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3nnhipcwa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3iedtwtto.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3eljlbgtj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3eikkcmnu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3usytbclp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vrcoyane.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3idkxbnhs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3vspikovz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ihakejji.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3cglrzqat.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3abwnhtog.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ltxpmgjr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uiayxrsb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qoqlboop.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3xybbyxfy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bdavvwke.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3tupkdmsk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qngkyoka.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ukpuffza.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3tbpyyfbn.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rfjbsgim.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zayvvxeu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yckpmxoc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hzposxmn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3tisjjglk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3whlamlhy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iyhgnwbe.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ettlnnsz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rxwjonls.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nouqucgb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eujkdaaw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zpnupcfu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iejznsiu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xweqetpf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ncuujsto.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jfacfviw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3aufbpsxu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qcmqfgsz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3lxbvunsv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xwhthyqn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dzrumqnx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3xbhoteap.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ikickitx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3uivcgjnj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3agfutjdl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3brrtgyqo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3obkifhey.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuqrlgwx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dbsemjxz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3awexrxwv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xslchurd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jukcbbih.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mdheuffu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jkjdmbdt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3xhmftvnv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tyobvcdk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fqwtziiu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wwmyuivm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jnrqqcop.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mmatyqqc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3sndhpzkr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kyinoirb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3tbobqvkg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3zqzygmjq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sfhgyxei.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fmohsfkt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3szxbgfbq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vpicqqll.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3fvqvvosd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3knkvgthv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xtsplbvy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vrazvsle.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3gemjeevv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zinkgzgk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qdlvuszv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ybmxyvfh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dzhhmtmk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3trctaxqf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3pivmpxcp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jhsmeayd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3sxmzbfva.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3cmpdpulh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3uxaqxjgb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3skxsyaos.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3opofxhtp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3cderyfyf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ukonprvs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3iropwiml.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3bacogqyu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3jrdozmbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kdsxetrw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ilxuoioz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gadthkfg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3orqldluk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3bvuxasza.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3mxaakura.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qotfizsi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkiuahdp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3lxoqxxpy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3byujoryk.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3sigocqxh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bagvzssy.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qadrphbk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3mnsjkqmr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvpxurad.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rqnriihw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bpbdbfjb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ajmashps.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3mgnfzqjw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3cdfutxoc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3msdrmzzg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3bhqgdkzo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vlnxlzcz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fesnimdh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gixeafcc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fatwldib.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3utdhryjl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tzemrxlo.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ngiioibe.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3giciykai.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3gqpkxwho.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3suvukelc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3povzrlns.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tsgotxna.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yttemfgh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfktrxyw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vwkkwbth.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cyjvstzm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rvhxexya.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3kvfcwwml.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ozsxssxr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eujkqnig.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3odymvazv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynhirzet.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jkehxcwf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3aetwzdmd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jjdnppzg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncmjxdgt.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ensydniz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3jzggpqeq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3drufbcwd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xxykswbp.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxpsvhwk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjmpfctg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3anbzxpez.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3tklbyhil.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3hebjdsft.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3zramzrqr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qolvkpyg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xhyaykfz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vspqfmjz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3oytsxaqb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3imwjnyuh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ersiseua.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xdeclgks.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wpysbpyf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3zpyxfqgf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3jgfbxlvh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ikuynzpp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3mpgqnivv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3dzsalnsh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3gbapqxni.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3lgmqyroo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3uzgvplnf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3monngowz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3bdxoxgyy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ggdmhycv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksnsogsu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3zycjwjtf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3khmzgfxz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxxajywa.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3zvthzyjf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3vrgbwnjm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3saaubcch.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3vwkexrxy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3mklomnbq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3scbatrrx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3aunfvwnl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3utrjfrwj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ybozzxjq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ynloctmy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bfpofrjy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3lktnjynt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3igytling.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3adtyqtmo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dywjmfze.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jarpycue.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnaoifqu.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugjcaynn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jgfwrlty.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3pooyqtde.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3qydpzftr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3swylsxas.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3bruzglkf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3czzcmbwh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dwptfirw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfpmypcy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rabxmixd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3iqckyozx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pnhzefpo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3yynubjhb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3spdkksim.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3oagaaffa.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3utrknknj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ozvcnici.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fzmreidu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3unyzawpb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3wfcolhcy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3rjnwvbiv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3bvwtxjud.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3eflthvpj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3kdzeyunv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3apynupje.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ukdpprzh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3wfpxmqau.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tikmkknl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3tsbvyspi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3jadrtnoh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3yultqqjv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3cpmsoukb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3urpynyah.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3rpahwnao.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3uvmxygmp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jtwzhxws.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3djawhpxr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3hyxreglz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3kdvjpqkb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ttqphuvo.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3yvkwjaoj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3qyqrcymn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3xlinrolj.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rofayjpx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dbltegqj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3kprnxijc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3emrkztyz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3topdeviu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3uiqmpmsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fatobxkp.html


<!-- 参考信息 -->