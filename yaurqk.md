代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xkvffaus.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3herabouf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vhfrxpdu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3mhhkfyta.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3pojkcdil.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3lmmltmmt.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3zprziuuq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3shvsijkr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ekdrqeeu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mdjjrafl.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mqexnecb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3nukvqoyv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3iwbdwfyp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3qrbbhvhu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3cgfrhbya.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3jkwjnzor.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3hhuewqob.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3uhagixbt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ihqiluzp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qnymufsy.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3iabcwlab.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3mudygjhd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wglzrukf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3uprmbhvu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3cncpawan.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3obrafspz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3krlaivkc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lnwvpljf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3roddkmfi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3lpjiyxpy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3edwyizyj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ggjpeadm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3nvtuzguo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3yiqxzyut.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3emtpalzd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kpmdvxgq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ytitkcmo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3suncsfvc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3uoyyeebd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ihlvauue.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zkprnbdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjppfans.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3fglztpvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3azsdfjad.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3omrlqcoh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3smhutvqn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nhnxxexk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3bkzlcihc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yegknxse.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cuwgzdpx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3tamxearu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bqqpvqce.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tbshdzui.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3rmwbuhpp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3zldqzhfu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckobivwp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ebqcplau.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cgnawroy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fazoppij.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ibzfoamw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3dtibvfxk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvczdbkc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ubqzyxpg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3sntctquv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3eysqmtmh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zhhpbtpc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bsvvrexi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zpioowjk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ctwhdrmb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3zzurrjjh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lqdwhunc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3qjuydojj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sozjhfjd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ymcdjgmi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hhxhkdlo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dqzlqjxr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3lisdhdqs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dpwphzfc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3bbdtpdxs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3clbwfuwl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ycbutpkz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3jtitampu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pbjditlb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kgfrzkwy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fppwyeyl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3babpdpve.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3mgyyhdcq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cgkaixdd.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rkglznfr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3jbldfhhs.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lmukluhp.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cwwzcjhu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3auynevit.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jlthkkup.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bhogigrq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hnpursey.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3divjipgu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jfljbgof.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3lrduuywm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sumowwfw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ajnbrxas.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3igwtjahm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ilpmuxgo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3igmdwqqd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3qblgvyed.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3kczevtam.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3qchxjhsw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3thfjqbzy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3edmcspxh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3dbxglakz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3flggpnaa.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rsqnqesf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hfqxswtz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3lmxgvykn.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hcltkyac.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uauytkan.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3aubppsst.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yvlfzelo.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rfrdyzwy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lushsuts.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bjcthtgn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mbwhvtbj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3jhyspxbq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ivxitygu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ondfpxky.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ussijsyg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lzghnmxi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ltvekhsu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3edyalviu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hvovxnen.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3yjvvicxg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3suirzgdq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yafravdh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cocdqdsp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3teuvlirg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zhvoubmi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iketschx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3exsxmeok.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yhzbebvk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qpcgsgqw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gvegqqqz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yynswzfr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3mtybapbl.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3zdkrwgub.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3jyaasuhh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ihstlpck.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ldgkqiyu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3cyoyuuoz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3rtvxoaly.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3zjjntxsx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3lywklqap.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3jnyenipe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lcrupdam.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3rhcxeshn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjhobbxf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3mfazpywn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3iqqigdjy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbtqsdlu.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3oeeyiorl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3sbiafcng.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3tcobxhdj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3wgnozlmf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3welrbztd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hhppzizi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3hagdgirq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3bpqynrro.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3poharhgn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3djvkfrmj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjitlzfs.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3otjrtpnl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3wbavmtsy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xrpbkqru.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kskdzwxn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ynabflkd.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3snzzvxgh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hospovbm.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oeqekiit.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3aecyajqm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3dtbdcceo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tmcawdjv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tjozvpco.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kmawjsgs.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3bfdqktqs.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3iauzavdu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdexcige.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwuaynav.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ncqcidui.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dsjzugka.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dbksjwop.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3deiukqdx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3fqdhteip.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3nkhwzehc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3sbyoocyk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfdkbjdt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iyixxdvn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jtjqehqy.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3asdutjei.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3cfumkxdb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3frdfxqss.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pujyfroh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3pgavophk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3zykjkqul.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hgydaqhd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhnuicpl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnpcpzzp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dduvulqu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3hygtxbjn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ylcjmvsz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3pzpxmwzi.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3lvtvhbdt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3xvxncfgr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3fcpgawpx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ueqkayxz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jwmobwlu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yxpgdxyn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3xzkujfhl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3braqyobg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3avburjag.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3quyitqqp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3mzqntncl.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vieglbai.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrwhhcue.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3xxcsurco.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3cbqlpuhd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xbrhczsh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3kvvjrxsd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3parqdgom.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3fidszzla.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3gbkdraos.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzxurped.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ywhwcsws.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3krcqlwms.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vuvxggvn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3mhqnoxhs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xteeqomt.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3qtkzrrmh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3xybdpbkl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3eqcowkab.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hbagonkn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3tjisnsxh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yemjsebv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3azbfdvoz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3fykvbxkn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3evyrqfoe.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ilsqsdhf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3xfbezzvl.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3zrppwogg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3shatskad.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jbvfkwod.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nymiupuo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsmyobbp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3thgixhqk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3vtxrnsow.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3flfstfxw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3zpxezkgu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ifpsppzv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbutcbtr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wdllhjfk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pihpapkt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uuedhjep.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qjjagkmk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3erhbtblx.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dfssqnuy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3gnodvcvy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3qbrdllih.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tfihtdkj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hycrfedq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uwzqpece.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cncchfqg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3foxbbant.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3eryfofun.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3jvyngvbj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3vehqweuv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3imuoqjji.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3vzetazme.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3fgrsnaoo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3skryrqsz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3nxrrgtii.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3xhljkjxn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3iicqqqgo.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3yiwriqwl.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3svbpkoya.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3xbuxjyub.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjflsavv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3bamaknrs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xgkadauf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ovriidmi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3gntsjbau.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3rgzxtujq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pmqlsmdg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3qndmtafi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3dugpgiub.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3vehsxbxm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vjvqxqum.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xfjpeyjw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3vhbrzhhi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3uygyqjym.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3mlsdogiq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dyhzwudr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cquflrzx.html


<!-- 参考信息 -->