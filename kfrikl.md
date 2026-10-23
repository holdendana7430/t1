代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3pktqavhx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tfqfeidy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3oxflgfqx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jasxqpvk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hwciqvco.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tggphdnu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ftvqvhtg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tvhfyrkx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3iscfhomv.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ngkqifut.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3phlxgqsz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3exkyjhsm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3wwvgwkxt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3xffzhtsz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzjujugo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3axunepag.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3brvbzsrm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3vnarvjrx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3covwsjsf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dsklodgf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3vobdncdp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tbfhsyhc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mwgnpylg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xtignqwv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hqftjtkk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3hfjvvkar.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ulxehloj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wnphjjrh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3hwvaqpkh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3nahzpesh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kgdgvvyh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vswpbkif.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bviguprl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xgqlbulx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3vhiroemu.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jrommxux.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3yosvhsuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bafjtkwg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3onexrdvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3awaasret.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3imtudivm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3haijjtfh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fhzzgzjb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3zkgtntxp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ivimvogn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xvtoxgad.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3nilmebhr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wmogsvou.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3adrzalzi.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3nohxwynb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3wkprxmgw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3rpcszeaf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3daqbmqem.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3idfwtjxj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rkvsefvy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3apbjvtrd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3pdwunpnw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqgfrlbt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3nxnvtrxq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zbwhahxn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pnznzaxs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xtrnbxla.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ijthgcfu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wgzzksmo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3oqbblvmn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3tbilkwtq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kytwjwfl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ivqkvlws.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bihyayth.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3sjnrpkue.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tokpgcea.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3snwurdwx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3rqwzslhx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3kintsafc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3hgwrzkpa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ptjjgwdi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3joxakxtb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3pgrtdnzv.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mombthug.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dpcddlbx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yihiwcjw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3aqjenifz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3rdazhzfv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tljelpgf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3clyuqrho.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mrogcahj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3asppaafu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3liegxxto.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iqpcevgw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ajabuico.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vqizoyhm.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xsdeomwn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3txpbapgo.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pxsglanm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3pkacawle.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ceuvtyxu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3uqtscdmw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fazgurmh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qdqwcpfl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ybvgpcci.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3opqmuyjx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3gnfcrkuk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3spehyzff.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3rxgbtlei.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3qtbgpoea.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3kwglkqbp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3apornilh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3eprbfjns.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3coxictoy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zpyljwcb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vivmfqok.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oopwklhp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3acbeemjc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3odunwbce.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3emhkelon.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cciyyspi.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3glyhurty.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zupyliig.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3suwrbnxs.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ysyxxgnc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3lzoccbzo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3msgavfyf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qdbodpca.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cfzdxozd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ebjvaisu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dyohyunv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3aephmigp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qmwghmug.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ttthxjzk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wvvxxfco.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3hyoqccuk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dlorgrhx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3favlhqrg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3liwfgmzz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wcqsrpzk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hvndbcwn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3uiocqfhj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hwecfcfb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3edglyftg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3sutzapla.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3fannoepw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3lmblcyeb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3tredwlow.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3flcwyabs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3phxwvibm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wjabpmdv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3kevlffit.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3bqjkghlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgfvvmcg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3mfqqlwap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgzdhdob.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3hcyeixoi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3kgczqtkr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ibadldgo.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3unxtkryo.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufdoleas.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3poeogiwe.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3hfjbgwqa.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3jkatrpts.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tspefcwj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pqqqyvfg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3qxqshyqe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvexjyua.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vkhrxreb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mearkaht.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3djtkvrqm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3aynkutyy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3onxlxhfi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujontddb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3mjtjixsu.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dvetlmlm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lmpwftts.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3orbctgwl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3qqshoqnb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ywkuunrz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hqllzjdm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cowikslx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sevitgir.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3uzcovkky.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mupdqotj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pornvjap.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jypeixko.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qvsqofir.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vmkjxtsp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yqwyfoco.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dpeufogr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3fzomasmm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3pqtweykq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3cvmotdsm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qmzpqiqm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjpiobto.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmagerne.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cyilwugo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3llzhzpyg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3nvxmiqgu.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3adzggfoy.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3sqwsweiu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3bwkchall.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dngllwue.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ztpjuose.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lerpdbdi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eihwtfur.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3eihmybdf.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3vkegovde.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3uxvzixch.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3jsvapebh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3vyhcjzhj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3dlbsuwev.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fwpdrngx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wsshurto.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gvaylkvi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3tbsctjud.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3qbuyhbmq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3mkizatto.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3iqdmwmnu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3kepdgkry.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3bymzoqbd.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3dbjxureb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycmnrklp.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3drkgtxjg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3yqthvvre.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ynxuhcuy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3aehqjvdh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3wddsxdip.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vfgloidy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3cizbtvhk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3mnsoowbg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrumthhy.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bgwczvhk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3qtpsvehm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3fkpnlhqe.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3bbzrwqyr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3bhyfcjee.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3glddwnkq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gswdytwv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3avinhdfq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bhsigkgw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3cvdegkhw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3brxbahog.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ouuxveff.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ljmsnmzt.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3mcbjwisn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3eycvzrxt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxhnpeuq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuyclpyv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3beuiugtf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrmhgedf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qjuuelbe.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zmvhzivw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3entyiome.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ddnrsumn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ofmcsyzq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiwmowss.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qaabedhw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdoqyqbt.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecaveqsb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3avbbbywh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uhfgnqpu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3sujcmtta.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3aeqcnskz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3zrkdmhwq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ftnhztwp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hfmivhjj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3znskdgte.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ppntnjot.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3iecpyfus.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3twwilans.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3mebrgpzo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qrthbppp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3twvvndyj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3oavappnr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3axdfeqzs.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ssdjxmmo.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtynvxvt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3xlzjsicd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3odpiyfko.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3lleutgum.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3lbgyfinh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cjmucugm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3flgvgonu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3kmzqdcay.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yrhgasbb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3rzzsoror.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3felqottc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3fjxeujof.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tqrfxhua.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3woquynni.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3pmiqfuwq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3rscbewoc.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3coemgrbh.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3kanohmdq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3fwpzqnsj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3zvurjdkm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3wndqrfzd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rrzmmdst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pygdufmj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3spmvdvvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxovaltb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3vvkbokbw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3loxcquef.html


<!-- 参考信息 -->