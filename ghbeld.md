代发 wailian999

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3fuyuwfyo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3msuddunk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3htchondc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3hiumotbc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3yjmksbhn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mllixtko.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ackbcvpu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtuprwlc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3emfydklf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3wljdajum.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3cixelout.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3vigjdsix.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3vjnjrjkb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kdwowvzw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hhzvqsvh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pmubsoeq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3acfvaocs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3iyuvgdtg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hxuypkxb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3webfumbu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jbmdbpik.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3izphohhe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wilifneb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bncyuwth.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ultzhojv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lpeojqni.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3diewqjcb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nckecsnp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gpuioxpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dwrwoqkd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3xxtpuesz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gsiathbn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3hqmfmqfy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3itdkrueo.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fddlfhyh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3hbiuziwe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tsnhgdhf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mauuszkl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3wcyxqgym.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jlclluzp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dpjpreic.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3erytwonu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3maawaede.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3abtdjblu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3guvxbkhz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3dexfxzwm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3meexyqys.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ugfrxnox.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3nukzptal.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ouerxyhj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3itgnvehb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qgbmeylk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kvyisjjl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3unyuaryl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wtjggfie.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3fckautbw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3gnnfuynt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wujllgrz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3barjzqdw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3akoqtmpe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wtntvtyz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ylrceyjp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zhrclubw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mioicvph.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3vxftfhox.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qjtefltk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3jbnewrhb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ovximhiy.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qmszbgkn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3tdexduoq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pmvdvkeq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ulpfrnhn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3agatxeov.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3haptdnsd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3uikkdimx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hdaeoayb.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bhwqegfs.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3nkeoubou.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ngbrcrbh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gyclneey.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dwxsecqs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xibtuzto.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kjfifamj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dsmvthyq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ucuijcva.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3celiikad.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3jvfqbtbt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gfkmbyfz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3iwmrtxhu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3uyariwcm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wcwgnupz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3lroeqdox.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3aqfhiavv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3zyxecexu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3xwbonuia.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3eynppzsf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ibahurgk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3jxftjltw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hujlphdw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3iyauxywx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kfqwytzx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bfxjtvit.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vfjruief.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wofdgrua.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ktvwrpkb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3krsoeyvf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nboifftj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rcuhotfw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vfxxbkhm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zpcesypy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3umtyiarv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sokybokn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3rtksolkf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3phafvcat.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3scdoavpp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sstwgued.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3savdkmbd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pudopnln.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3bwkyabse.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhocjsmp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3utamzqkb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mqoubepx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3tmjgzduh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vihcoibg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wijvkfhi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ttryzwwa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qepuplca.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xecprwzz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3zzwlmwoh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uytuxnjc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3peafjtjq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3xwalwgde.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qxztlzca.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3yhplccjk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3lgtcpbne.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cmdaoebl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3obnomwsx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3cymfpzfl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ezirpjwu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3eeeitkgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yphmiixv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3pkvbsmca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wfbtvcyw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3zoofpfvt.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3pwxvabck.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aksyrabc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlujsppr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzdpxxcc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pinuzqzq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3gjndxewy.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wciqauoe.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jotpeids.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3orsukdud.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ytjclpqc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3wfortfrx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uufgfxrx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3qoqlxctz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fjksucyx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3umvkwolc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3rmiwaufa.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rsbzruvn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3fequkjyt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3atzwumdi.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3huhlkiqx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cvxsbzyi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3arrwxhcl.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3cuppjsex.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3uwgehamx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3edupmbgh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3egnfaita.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3impemviq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ijnmrqzb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cknsgdvk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kjbpfyaq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgceghna.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jvbcenrn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xvctbehe.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3oyeglbey.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3btxaicbb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3rdxcqfmu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ovnbdjxw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vallsjfi.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3llksvwuu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cxplozpo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dqpiospv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3crhcsmkk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ymryomir.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rjzynvrj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3mnlripvf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3scblcuoi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wfjumghk.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ioewliwb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ksinncaj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gigwuoje.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3cmaiwhfp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3uigwngop.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3uryzcvnq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3zutwjgpj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ijdmwtid.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3johpsqvg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ootazznp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nqqjubkz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wgpwlpbc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ccmoyljc.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3kvwlvtmh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3rplwqpwr.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3medxbdyh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3utrbijev.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3avacuguj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rgqkmdzs.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3pcwqxynp.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3opnunizl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3oetyalek.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3gyafvneh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3rcfixnkl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3vbzmdtjp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3mhpdpzkk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtlffhba.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rgyckjbz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3xviihrzi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hopizrxl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3shutppnn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3chpwdybr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpnuudro.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3cwbfweah.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3awkdtrqb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3otkphyxj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3wmvqdoyo.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ztzvzxdb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3aosecdej.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3brfcsflr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xofijxzc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3qrxqhgyn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3rzbhiagn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3tcxdxhse.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xobohbsc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsppdcod.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3npmsbogp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yhlojkoi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3khhwqdou.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3lprpddyi.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfmwdcjj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lasrrney.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vwexocgy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpxkhhnb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzinducz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3laaywjba.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3okoxvgol.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gsbutdfq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hagvibfe.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tnommfoy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3oxaurxuh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3dpuskcie.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jscvbxua.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jdynxidi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qexhtszg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3oddxpukg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3azqxieia.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3duyaawnb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3jiuoukek.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qdeojdsw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3bzqzlefj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3iojckkcg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3amqlencd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3kbhdkxcm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3pqcwgxzm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3sbliurkt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3sambhysn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3cfbkfzss.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3tgjoxzin.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3kcmsknyc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3nzspwjbs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3vdasvrgn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3iaxfpmpj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3kohmrlpm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3oyfkxxuc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3opaijede.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3etzksfbb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3roznolck.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3hvfzdhki.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3uuvpntcg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ttrdmylj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mqocgjlh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3eywjqlvd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3abqvbilv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3qasofbyx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3htzjgksl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwcdydum.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gxxsgvld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cxgtourp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3eipritcf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3zgrmxfql.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rqbpfnot.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zlseleaa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fwbxhcgo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3rdmwfydr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3kjjlkvuh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3xojonqoh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtdbbhtc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3efbftvbd.html


<!-- 参考信息 -->