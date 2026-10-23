代发 wailian999

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3tgqmedoo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3onnsvxtw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3hbnbsqgg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3palkstzf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hjkfsfly.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ypcehfho.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xarbacdz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3tbymmuwz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ynvynerq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ifbssrmt.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3mrvmgscl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bjsnmoin.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pxcvfbyk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vkforuky.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aziwqyke.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3gaejccbo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3brrrewpt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3gcaxyvgp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3tqmaxwmh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3jqrmljkj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3etampdbu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3pmpbetvp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwsrjear.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ciijkovn.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3foqqrcfj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3dxynkmcx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3usoxwkqr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ybnyudxr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3zdrqwggx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wptrsyam.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iomtqjrm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wzkrgfhb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pgecvjcy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3jayjzsru.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mdelunlm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nsqxsile.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3tzrubsgi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3esagfnny.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ccefucei.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3obgvqfyy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3snfrvaes.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lgulzdfm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3yqfqhnyw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3caslnbcr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3murxiheg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbwexecd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3irbxemzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndaftpmv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lofropdu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3aogweewr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hzvdwhzq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3edozyjei.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3htlbhywx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xilutseg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3mrdexubp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqfginxz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ucfaquuw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3etjcwbap.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3dbjmvhdy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3vkpmdxhm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nlfeyqth.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3phlbiibz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bfhllviz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3rfjngzgh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3xrazdwbx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymnqliez.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3uljfzrws.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3wpvotcru.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wxqxnnzs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xiokyrnz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vrpysbwh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3swhhcbkv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3olheabuk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ddeblqyu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qxdtutmv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3rhhgesgy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tcibfjca.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ewplyddy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3olavsajx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bvikdilr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3szgcunfg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hdszceji.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3pchcubov.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gpxgmllb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wvornate.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3hsqcariu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mhszkixq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oawfgfgi.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mfpuduhm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3druzotvd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ruynlfig.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ixtivxxl.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ivkwnhfq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxzfzull.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rzqrtotf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nhzrhoce.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3syqzjkoh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ongdkuzk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3axqihqcz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oqjykegb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iwcuzqmy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uyriswaf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3wnaorjvv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3thiocckv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ofqrfxaf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xnssjqbo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kwmvxmfe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3oelxxsut.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ubxmviqn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3qwwqzlzs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3bkbddshb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zknguhwy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3mxgnvbsh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcrnoooo.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kscwxyzo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zucapsvc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3omvvcrnd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bflphdng.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3mtrbulhx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3kolbsxij.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3uszexwsh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ahxmuetx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lwawkmvd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zkrnejnl.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ogtqlssf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fmrewdqa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3baivaked.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gynculbc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3tmqexfhj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3vayjumvw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vmmttxqt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eymhpwyu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vdddiodl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3heizykmy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gpszzdzg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xddyxrqm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uqhdpkra.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rrkkkhyk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3fojogier.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3itohnelq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ubrugvcf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pazyjqgi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ileyvoys.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xddkcsct.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3bhfwfetu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ohforntn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3bdqlubmf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3vgtfvwze.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3yjxnlnrk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3nnqxgejp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3atsmwtqr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3indvnnot.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ucrayiwb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3umxyyjeu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3gmirmvld.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3rjypfqah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bavwofud.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3tzoptxlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqwdefoa.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3yynwibrw.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ontoxsbm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbgohfwa.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hcneuhas.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3czbshrzx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcachwjx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3frzahpjh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3tcpzbgwf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntvynavk.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ffwkqhfg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3qdkeituj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3djfffiit.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bufeaejy.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdckxbqp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zjrasbol.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3wjxkzmem.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3hzpbfgse.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pyxdshjt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3osgdrczd.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zexjnqpk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jikntatp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3shgkxroo.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3evycbrmr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3wqmijvqt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3otbvnuhx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ccvabieu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3suwtfhec.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3zzjtpucs.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kpuzbkjw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxqslpxf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpsbpopi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eqkenzna.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nsqsurha.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pabvbhyf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3alhibokg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hiljkrmr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3spmkuctb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3eoaqyxnt.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rjtsbpfp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvvkmftc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3deedfbjw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vkssoqni.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3bbnppwzj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3bvypjjtl.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zskmmqdi.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3icjxbbme.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3qynbriyc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3czxfttrq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkbucysh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3akyvkifi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qynkpngc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3acpiihkj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3cugnfcku.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ljgidjku.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3wcqtmpno.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3mqowpewg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3poxvoser.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rpmnqrsl.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ipxxivwb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pneohqkj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3eqwbcqxi.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3jmpdcilu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3skuvvlbc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3yurzqtaa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ywwuyfdb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3wdlrbapb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrdrsfhl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3yrsthele.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3bkbwvjgz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xgtxpaxo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3fzbucxhq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3svrvimxn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3zxqeciyv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ornixctf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqlbphct.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3pcghvoxg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3zejqwqpz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzapllge.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3gdazifaj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3friurizr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xhmelwre.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3zbfhknzz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3qzrjhtdj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bvktbjvx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3cwncgaee.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3elpjztgb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ivwhrdrg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3zsawqvom.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zuirpyur.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3utbkozwt.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3kljzsyfm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3gwyyvjfu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vsmvejur.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fbudbqpn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3itdgmrqp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mukyvmta.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pwnkwhca.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3iyowyynh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3pmlnrztt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3doxnqtep.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kanqyfpr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qmaoypxe.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3onwpdusb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvalcbvd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3maxmhsfh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3smeeaciu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qiqyinnt.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kyfalwwj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3mmttmesk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3fkjtweyo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tfsgsrqr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zghmcfip.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3iaeolksz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qbrhlzny.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3wlvvmeyn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3snmfrwzl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3yafrllgm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3lpnpwlwu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3bwjdvxlu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3zzhoqgwp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3mckwzqnt.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ldhmuomv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpyekgly.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3zooxnzyb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3pdvuddix.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3memhjtev.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cekovhtp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3uuejcsgo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3xnhclpzd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3bzkbmjvk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qvrkjhpp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3vdgdzmki.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3tblfsilx.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3lyyiqcdu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3teljvgoa.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3nsdqtoah.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3gvlupdqe.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3steoevdv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ojuuocpt.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3kqbwutmg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ekhbanyd.html


<!-- 参考信息 -->