代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jxibkgic.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hsathnyc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sxrppxbh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2apyfuzex.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kxayxkyw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2oczrhlhg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2tdnalkvg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fmplomra.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tnsvvhfk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2beoyvqlu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2hxqbuufs.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2vwqdddyn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2yosrqcym.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2bjkayuiv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2rropcpiv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2vomqlvsn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2mpgyrlgd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ylzbegtb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdsctpcc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwlpsrsd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xkqnyvkg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2schvdecf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2vxcrcbwx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2abrskqhl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2dwiidqpz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2loltqocl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gvamtqmq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2prjirtgk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ulffqvpx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2angnotmg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wbfauyvs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rojmcpmr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2lknjdkss.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gntpwmdx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bjfgsgiu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mfqgwiiv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tenkicfv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2aowyonoo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hiktptha.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pozdcptz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2chptfsxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjatrald.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2gidredzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ppgpfkec.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xbvfxfqy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2xfafcajd.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2omtocvky.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2jrbkmzgr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2epntyjdr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ljdfyfwp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2pdxnyetz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvglhils.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2glvgcsrf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2eiuaxivn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ncknxrzg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ticsbotv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lcbsgrla.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ombvxgws.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2bvgvukac.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2rkdycnnk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2zccwtkoh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2xvuhtjsn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2rtzqfrfc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2diufbsam.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2yebhibrr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zopgkfdz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rsbodbai.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zenjvceo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2rceyqbji.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nwtglpja.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2djchoitc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2zbxvtoir.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rxinxdrw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ycvrcihd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2adazenif.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mxcadxfo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2uevmolbo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xflkqopq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2znyiprbw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2limrgocl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ajswcahr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2uqidjfny.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2byhmahcv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cbsouwph.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nievruop.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2weyhjapt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2mgbcsbdn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sldcjdyo.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ivamuafx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2kfrgjyzy.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rmqjmuiw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gcpbelji.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tamlykwz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iolqgzur.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tinkzyzb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gxlqqhyl.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2elzkgavu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2drspbhpv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2wncwcdvh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wozdcdnb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jkmfqiui.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2emcqjayf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2aercrjub.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2irnljsyw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2bvbxkwiu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2yorxgmry.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2gofxzlog.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2gterlbbh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ousnuqju.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ikcgbuik.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wqgfespp.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gjyrhhep.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2txujcepj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qndwyepc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ppxgxwvv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2stethypm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2tormqmur.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jyrkyupm.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fjlvuiai.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pzhxgivn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gpcrrlrv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2epvgxeop.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2myiezctq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2djgkpylz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zxkbjrrg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2pxjuyugs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gpvvmagr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bcmiwwae.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lvdqccvl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2boxowcyu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2moikfkcj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ypcoxphq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ssptiwbo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uhserryg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2temouptj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2guwtabsd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aqtefngn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhobvxnz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vdyzgujp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2drnphucx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ldopvuem.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bzvpetvg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2cdztehus.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2abieytdd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2dzgwvdrr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2lwwfvctf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2whwsoemb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xnqpwhhg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2fmcyvnxl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2nuijdjrt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ikjgozxj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2rssctbcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iuvygkvr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wbgsyebw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bviqjynl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2atopwuwb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xjypfyig.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2pcnecfoo.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lakfpiqe.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2mplfyguq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2imcffnmv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2cwbgrooh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2bfjcssab.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2odazfric.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wvfjaaod.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2htttooqd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ztiycnsr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2evtgfgel.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2hrjhdfls.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpzvbwfb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2nbolveqh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ermgzqqy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rabpswhp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2flcfgxly.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qbeaqnrb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ehypxpph.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2agymlnhy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2yiaepekj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2zsfajbzx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2iujmpxlh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ngwjcydz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ynsjukrg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2lsxqmubo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lixozwlt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpnvvyyc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jjftrmnm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pejoftxd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzuimnnb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xurwvyhs.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sbopntke.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uyttioxh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ucdwzbyx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2vhnkbiid.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2puxdundj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbjjnnxs.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uaedsjqe.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bwgkfujo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2crhjssls.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wlmgyajv.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkkkfdwm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2dmxanlmt.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2jfxckmhs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vdiksidi.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxityggx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xvatrdnk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ucnaqhll.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zvjiuycw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2wlhrwyyf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2rdmpyxcu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2gqrkaawb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xkiskybs.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2fcwfdwwe.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ibghtlst.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jqarlwwn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2akugllfv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2aofnfkgi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2yzvjmpay.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dijbmesn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2vbfhnmhf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2mniczhae.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwpyxtos.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2aqewvpqa.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmvyxhyr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifmvrhxa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2nqgdruyy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2qjixsqrr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2payksati.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2zczftsuk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2vtctiode.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2smjhcssu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2lkutpsna.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2jgmfeqgc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2yoytgxyi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2cwsdjolu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2dqmpobuw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jaactmgd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2zanamquc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2zsobryjr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jjogpxsp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2saugiuji.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fnopnvui.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2dfihwlim.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2uqudohlr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bjllueav.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2moveomuy.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2pvnutzrq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2dgsyvuwt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpfgjyiz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2uwsyfgka.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvdjvtmq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fiixabzz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yfpulair.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2dwubikbq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfzgrvbm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2kgwhxdqs.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2apojkjkc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvsudpjz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hwrkkbaz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2znzlkydg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2togokssg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fanqihsm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pkhkqutm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rqjzhjgp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2uggtxtrj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ylhmvszc.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nurnqlvs.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2untbvrek.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xuccznul.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ldhgzhyp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2dnsiuxdc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2kxfwkqbz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2fmwcjesb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2pjmcwalu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2uthajhol.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2smovqccj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2kwopqslw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2lbyorome.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2rhydnrhy.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2urijdgbo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2wuyvyeul.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ndjwkdqb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2twuhqefu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2mslbvxxl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtbuvjay.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2vodkrlgx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zmsyoljh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2yzqwndma.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2mimgqexc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2nrvakwcf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2woauinym.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ocywihgr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2atltfdcj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2cpbgkhwr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kwsaewyo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tejajxbu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ginzebwu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2udjthjnc.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2nrnufwhj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2pqezsfdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yczswkcg.html


<!-- 参考信息 -->