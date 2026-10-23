代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vqthkcer.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dbkmxdty.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xzzyxyrz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hlvqskag.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ovgaauwc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gvnmxvmv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3bjnzrvji.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tzmtmczs.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fakfmpbt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jxpzsvnv.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ggpdxfha.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3hcgkrogt.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3mizwezio.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3eushiiyc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3zqiisgcj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3pexqyycu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3vicuwiph.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzsuexkh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3bzqvhrxi.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ytyvcndq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3yonwirsr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3nqgvfcvp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3axkybxnp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3yuetgjwo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3nmejubaz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3modmxwwm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wcgzoyrh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ztxiniug.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gvdzdmfq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3wkjxgmpg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qgorgurc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xjinjgbc.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3dpywmgnr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vyisbjzw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dqkronrl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gcglscjl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3luemgnsc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ewcwfmyi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3yvdogsnd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wfdgxbvw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3paiqhtlq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwpgystb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3tmagrbrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exqevalv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3eujshqfu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3knekfdid.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3smwujegz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3jgcqrfts.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xrdzoxit.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rdzugcrm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3udvdfvng.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tnjhlumr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iunzccty.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3lwealvrf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3jjwwzxuc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3zhymdyrw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcvztvnl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqenbzxs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tmlrvfbe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wyspprmn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3pykstcru.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlxaubfs.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ubhkqceg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kldrhblp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3tljlgqiy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mrlbbiwl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ajnfttrb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3hdzhfetl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3vecxutzo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3xeiwjicu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qwptanjn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3exakesep.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tujgtvsc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3dvduvdae.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zvdaewbx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tmeviorf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3irewhfnf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dclhlxvq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3obrfdsmy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ybwdylhw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qerlpjta.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3spfpepcs.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rnvsnnpw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tqyaewrx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oothqyww.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kplgclhb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ozwezeto.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bntcygok.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pucyocao.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3kniidjsw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zjzmxhfr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nhebyhec.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3osxyvyso.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vayjpyqe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cjynjksx.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mwexcvsz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lwaryxas.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3owfkigqg.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qnglltpl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bbnpxodp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3zmqgfvxw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3noamwofp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cmqxsdpi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3htleigde.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3jwamvxpk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3hexqydes.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3osannjzx.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3bqwlxkbo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rlpcghbx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3sxxfaycx.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3lddhcnva.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3eqnllydy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ropzbipi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fwtkfdqd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qrqhigss.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3uvnyfytu.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3sbwyhmou.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qgyokidx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pmncwaek.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ydhuzryw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rhliqxjh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3chmqimog.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3bzfvaray.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uexifzya.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3htwerknl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3wiibsdlm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eokiyohf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kwextavm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gitrpkdh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ycrlvnxy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3zbzyrjmi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zrrocieg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qvysuspc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3muoxyhqc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3olaycann.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hhkbybsu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3khncyiyb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3foymfphg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qgbpptkz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jifioeas.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3nqwsakjm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rmuoamvf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3bjqvhosg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3zgorvggj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3wwqmsybo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3pfttqjdf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3bocpazci.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xjiwbwcz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3wimilymi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3zjtnyqny.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3innmwjrx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3yqamrvvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvwualzb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3gznzgwow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iahnaeip.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3hqfwghqq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ghlwqmdn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3humipgzx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tayilfkf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3kklrledl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ghvwaqxc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3cczcmztd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3dyufymrk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzcoqtaa.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3kcesvomr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3bzioaaoj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sozbmcyh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzeaetpk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3nqhmcjgw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vqbdizxs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vrersyzh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jvjnjdgm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwkipsjr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3btxldjso.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kpijgkqu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ppbbdcvm.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zjrgdmcp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ycdkypte.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ewvpyszn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ifspvjbd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lzumamqh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pocdxclq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3hpyyjoup.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ggztlulj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ielofbdq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uepevcoe.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qoxbfbbu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lytvtoek.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qudiehmq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zvmqdpgo.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xdydvlll.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3fikcchvs.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3mgjrtjhx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yobkhxoj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bdvooixt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pciobvjs.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mragurbx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3yjjdmjca.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3istschyt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqnaabwz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rkprrfri.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3qyrkrbwo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3eihxvwxg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nwlhgdqs.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iugaulpt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oxaynfxg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3cbxlriyv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3vusydoqi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3gspcqalz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3kfbddqaf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3buguzkgk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ufpfqxjt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nmmsmxpe.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nfazfgxk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rqwtjadh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3starfqtk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3yqomkgxb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3jsnoxjtm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3etqhxrza.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3cxwlzhkj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qewjdlbw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgqnpxmn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3qxrdzqlx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3imodwrjo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3nbogalbv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3lenpjclg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3wqhzqxrd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3wsgtsgtl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3khgmuasa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ouhrxmjx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3fbdyvlxx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3fgygnfir.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3vqpceqsm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3cqbwtdcf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3qgzixdwb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xitcaxjj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3igeuqlha.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3pbwbrwil.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3legbkjdy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3xqjeahcu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3elvxueyg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3juzcgclq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3gniclxou.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3awoylnhn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ppffatoz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3quvuxylh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3niljdggs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rayqzikt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvykrids.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvaydoog.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wtotjkzh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mefryjjf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3vcpblgnt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecbbxpww.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nrqthsvo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mitxifpr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bklmehgk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojetioqk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3usswqdii.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rjjfkbyb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xnjwhfjw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3dpfvlooe.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3skhbeayc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3enonnegg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3lfrtppqt.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ovmhsorn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3voroygwc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gjrzbegi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3omwxdimn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3rejvjtru.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3xqeftcbg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3hnnvkqqr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3byqohetr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3exqxsbig.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3qgetbmfj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3igmcdlpy.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3bursmkzl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3baqvkows.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3subkyxev.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3mgmmipwj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3zedgqqhy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qpdpldkj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3juinotqw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3nhisxjno.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3desrjowy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gtixyxkl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3uhjhfeft.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3zzlpogdm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3igcixbev.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ovvfoypp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3hvfqouvi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3sskvmuwp.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3typqsxtl.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rrezcblr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hwxezwek.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3szocfuzy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3evchskzw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3odevvwkn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vpazklpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtmcdagz.html


<!-- 参考信息 -->