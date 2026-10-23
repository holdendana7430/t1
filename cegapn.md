代发 wailian999

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3lzgvqpxi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3jdcguuus.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3nhxdxumx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fhdnjnwb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ahyrwusv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lzhvfews.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nihhisaa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ogdwbftd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3urrjvchx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kftbyrdp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3trohcxyf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fqtrltex.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kyenrjwm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3eqxjxgod.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3srvggxfi.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3riisduxn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3yllvwfno.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3quznotuj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3qtgaxdzn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3aslfintw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jpqvjdtx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qqbknuzo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvzkmmps.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nubmzojq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbusoehl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3rdtvmlmp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jywdlukz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3cbglpptm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ehkgjcmw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zntaqoxl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eaesmkre.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rrodpfej.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qhdthtih.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3tmybnvvb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3premplns.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nzixkynv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3vqllngqb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aedjktju.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qinsvqqb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bvkevfaq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qdusdawf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jkppfshg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3oxuqkqwe.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3orticreb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jbnxwzor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jybqwmlp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3eugpzkgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yitatwos.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3pzsusatb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3fsuuogex.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wklotbbp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ctefuthf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3keumddxu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wvhvdeqa.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3akbjtnyg.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bepbtaen.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3delxashr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3zghkwiep.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ivimwntb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzvwqcfv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3sqtktwel.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqcwvndg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ycserskm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3fsicqzxj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3qobfiamh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3cjuxzacb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3zacishba.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3oplntzgj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ahjzyepx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zbpjquqq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mibqqwjy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3bvfghztu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3cjpkgqva.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ydhmzxgb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jouzkpdy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3qettvxit.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xbxmmgzd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3pjngjlau.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mbtxslnz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rkrsmnzh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3vubohnaz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tptnrawq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3hctkpidp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3lmqlpwqe.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3iwrpfixe.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3tmbkptwb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bsvtqbla.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jmxduhou.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3twouwnja.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3aoyblqsm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3rozcvgvn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbrwnrti.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cipnfswy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3pdtcmjpm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3khgpgrbi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3evhceree.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tfelnlky.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mmocostf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fktuposo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mhphqorf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxftgdjd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ogzwpyxh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3tyxfgogo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3srjxppkc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3irjwpsfl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qtuggobg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wmnkqvcy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3eciwdobk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3dusuwuaj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3bsceegtl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3yiigvest.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3jjggbxxq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zttsmaff.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwgtublg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3usldlaad.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zgwhfplk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ieolxcys.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3yrtsthdf.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vessajkj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3elftgrhk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3fyavnxod.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wrsindcu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xsrrztxa.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3oltdjatb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jxdhdkgo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wacrcisg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vmqlmdak.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tfmtknat.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3tsponjhp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3sabtomex.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3buqndbma.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kvwjuqmm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fokwwkbx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3felgsbnc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xosmwkmn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dnlbfhbt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lgxlbktu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qaeoctuj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wuseeldc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kheznelu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3gbjszelg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xnsqewaa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3udyulayr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ebauhcdh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3sfbfqbnd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nywqroxx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3beqrgqwx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3glbranir.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3mqqxkgml.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3fprkmmpk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3jsbfwsfa.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3pvgetlty.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3uoolzutk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3tbfgzeub.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ptghhkxv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3cjqscdgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iajozbbh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3dtmlqcmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3extyixvz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bekexzig.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ahxbpsze.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3usoqvsjt.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3axkvbpar.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3fbodtiqx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3jbrxgrmi.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3hmhkcfcd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3pjrvekaq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3esuzafrr.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3bnizztvm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3gzcodsda.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3mchcxjrp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zianjyqc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eiinzbkx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3peiplmmn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3khaoidvr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ftawenoz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dqadpati.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3dlqfaavh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3yyhmajpm.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3kthgijzl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ckrqymkx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oulmdhuq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3oehmonvs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3zjyxaqpq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gawsfmaj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3mozrcsac.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ldecbykg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hsilxiht.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3divzwass.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iuwsjwvm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3csjrdbib.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gdmhshrs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3swwsugut.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kanrvsze.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ybfmnajk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ewbmxboy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gcylhltq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bqizmtxv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hbiwuoxh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzfpehnc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdeedfvk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3igfyyflj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hrpmgdtk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcbjkeay.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bytelphv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3fyurhfgi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vdgxqhbe.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vwrmhtge.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lnmttevz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mzjuhdek.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3uacgqzwh.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3dztuklur.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3dljxelev.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3uuucrvbf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3gzxvxope.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3relerkfc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vztqirfn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wdpgsfet.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3njunqhwt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3jluefqip.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3zkdjdiiu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xszxkcya.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3rnfdkata.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3nndckhqd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3mutdotuj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3esriwwtp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3dxjudfmk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3xuyglpxe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3hqjtvsdu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3egrtnorw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycsrvtzh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3tuaiwfmu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3sidcvsot.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhnvgpkg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qucxbuel.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvfwiteg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhbzvbvl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3zirunayt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ynynxjee.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftwhiogl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3xuulxuvj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3figsfhzt.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3roghvfrn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3wftzbwcs.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bznfdckz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3pcqjodak.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3txmwjqbd.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yrvmnphu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3bahivvwl.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3bqtbliim.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3gkjzodfo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3epdygbwl.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3lckbiyon.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hqcywqmd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbfaoaps.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ehxyzuzz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3wauciimi.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3tagfjxft.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3dqzypcam.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3euczrjsc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3phxkqmol.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qrlddkut.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wzjfjffg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpwylpoh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ypntzrsl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uzrcwxxf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3axdyltbg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3igzgjxvx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3znvuuaix.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3edohutal.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xjwrdmnz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3umvnmghu.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ddhhavnd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3thjhkyqi.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3cyejlbiz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3uorwsokf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3wwjnqqta.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3lzienwme.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3lqycyixy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3qhusbycs.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3nyzabige.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzyvbpcp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3cbjlzbmr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3wonrpsgp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3oqrowdim.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3gnidbsbb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zgcofidt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzjdofgj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3dxmmqhyh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bodrltef.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3dyaqidkh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3sojbkruu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3rhtlsqzl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zcitsruh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3lgxbgbpi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3zmtjxjvt.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3bnmvmsvw.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wwdiqbjz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qbxuoyqq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3dhzzoygc.html


<!-- 参考信息 -->