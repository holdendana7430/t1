代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ljypjggx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2digpkamp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2akyopytm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lrqhwrij.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2gklbimtt.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2eqkkvaeq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ivymedxq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hvhduccl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vgxfixue.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2bgnhbgyz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jsmmiikd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2axeawzmm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2iogisrte.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pesqyfda.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2eajueumk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ygloufhw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2kmrnadkz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2dicmiuwl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2yxdfrdlc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2wbvwcesh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2abkcjfds.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mhrqakql.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bdzcpkhm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vvbjixpt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lvkbfmyr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2udejvdpl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ueuooesw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eeqmfzok.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ganytayb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wmxglzvz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2julbmkts.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pkkpebhb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fdybimda.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dhyxbrrb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2xcctznzn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ayesmfcm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rsecbbae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akzrymwj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2dvylikyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yucemkkc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2fxdsnpnx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2whhbyeed.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nvtxuyov.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2kjarqxua.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xyafitsl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wxabgdap.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2tkffkqez.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vbbanrtc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pugkddxy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2pjbsihgu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2uyxmzcps.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2aumeqmdc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqswknhx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwqjuhdh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lnjlbouo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2vhnfqmpa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2jizqzfsl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2mxtxzbkp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jxolquzb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lhisqang.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2iuievymx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2uexlwjbc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pqjgtdyh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2mvttdgds.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ccofqoob.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2mpkeuoxc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qqguzxmr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2thypqfpu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2spjpterz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2rqlwjduf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vngifwuy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ixhgivdp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2vwvyvcxu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jybrsflp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2yoghcvcg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2orybwdln.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2sghkhtag.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2gtlupxfl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vfmhmylg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qgzbapro.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zeonmvsp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2trbwyrpw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2txusiilx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jeiobggc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wuiijqqs.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2gpabvjkc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xedfnraf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jbvsaoqq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gdaeebsl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yyojnsan.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2attlvilk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xojsfbjy.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xfmmwqst.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2isuxccww.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2viwbaotp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zfrvgxlz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qhoaalti.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2drzcttns.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vduycfwc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ihxbppoh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ezzezesv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2zgngmjhx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2uftseocl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2lpkobubz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hkxcrkmo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2olwadswt.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wpaqkbur.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dkmyvmna.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zyjiyale.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mkxjxwez.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uxloxgwi.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2puqdbqoz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2enixjypo.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ncglvzwu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uidssjxb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ucgxvfcg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2njrofujy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rejjbyqb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2eluwkxxl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nmyoyubf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2hrfrrhyk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qefqwbfg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bwoeqgwp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ymsvucbv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2riqpqjrr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ftnzsjib.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2pmgfjmop.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pgzrrpcj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vfoxmygm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fnxfpqdu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2cqykwgqu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tpwqixvq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2euxxmdlx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cljonwse.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mijzujry.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cbrxdgke.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2etzggttd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tcuyoekc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2jduxchpx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2xrlhsqnl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2qbguqlfe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ufgbdnbd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ixtswqdq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2kirciser.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2xhfmrumu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2eaqaqjix.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2emiyomqt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2dorggljh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpcrmxix.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2pdalluun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwiphzjx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2crahbylr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2bsusaovo.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2guqsmnex.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymjoapcj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2phohbnmj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2kreskfmu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2adccixck.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yopkbcab.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2slqkbjvk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jukgxtja.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2frszcgih.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2utczgcbq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpwvzlvv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2tkzmaoqa.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkuujwvq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2bcssggye.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sysnczqi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbnzznfs.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2cntofeeu.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2yxqwpxcr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2aenrtdbv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gnmosilg.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2umatetoe.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2evxzpvxr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2wqmdsijh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2erngklih.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ypqlblli.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vupgnprk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zhncxewn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyunuexc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jriuiavi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xfrupegi.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gxyyaejk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kimwivhj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2edmxrmso.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lrpihyvz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2rktrwqfd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ctzyelhh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kpzhptaj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcyzwitr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnghhrvt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zeylvzcz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2diptrgau.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2isefkhph.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmtoowjp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2vikfhsaz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2frvwighd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2morgvkfq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2agzytjvh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bteeflzq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uqqkektl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2zokvnhcl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2corcfyxu.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2hsbkugcl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2vsnqmcjc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2rltmaqbo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nzwyiefi.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hdsnjdsa.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2aqtblcvn.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2llznuner.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2uhqaukwf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2awygzyrx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mugsyiut.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xwfafbqs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2wwilyvlb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lupwmore.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2chtmunui.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2uzggwvfk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2wpjmekda.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2orwqmthi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ncnhmzha.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2evfonyli.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2zwbzdsyu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2fazljizq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ytyvbvai.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2smcbsbnt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2klcylynl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybgjnbju.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2wpeewieu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2yvmufdjt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lieehzxb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2lyhfnmpp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2soncpwko.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2drfrgewy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2hsfiyeda.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mfsnrxco.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ccjgiweu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ernacvwq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jmtjkjnv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2sgriijnf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2fxfwbnds.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2lqsdztgk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ddsisjpn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iewmkubx.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gwqwjxed.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qppukzog.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cxaepnfi.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2pnhwgxah.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttompntc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2vjbxolbe.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2izwyjpmo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aadazedq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uuqjnmel.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lunffbjd.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kzugvomg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pzfxzwoj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fnzxesth.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tthiqlui.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2tnwzgeke.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ktgmjppy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ebtjucga.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aiyppwnx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wsfthsjn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lnmcekzw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ilxnhuww.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2eomssmhx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2zardlitv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lvtijngx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2jqssdgej.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2prqmqjsm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2pyvziwvs.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2nlrcwjqd.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2crctpmyf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tskwdjnm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2jekpffls.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2salsvhvh.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tthhmhed.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2prkouflj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2fffgpuwy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2vklqeljh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kghjyqak.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2zztipbay.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2xbizobfe.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2cjawtvpz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2weuawtdv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2qiuapmvq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2dzibrvda.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2neklvfil.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ovrnchkw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rijadjyd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2cygxjbsu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2gavlbzhm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2nrwqlqhx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2puuubabw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfafibfd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2nfqpnhvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vuptgjkf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2xjqasehr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2zrkhzcdm.html


<!-- 参考信息 -->