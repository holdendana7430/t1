代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3xlhmnutu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3nqxjjypc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3hmhccmgm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ntnrqtzh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tqncnhmm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hcvoudzn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3zmpjujan.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3beijpbwh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3cbriajid.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3gutsnjyh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3scusqrej.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3alkuxknf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lkwqhbjz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejotqoom.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3actljshk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jljwtewp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3blxjikfp.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3yfmyahwg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zohvrukq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3kmrazjnh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3hhnddfgp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cluewbwn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ajgjhxho.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xvwgjtkr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wmysmcnn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3axusfpav.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xbcostuh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xblyckah.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3cjmvyyjj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ubkzvnqs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3odjuytwx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kchigfuw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3iozmfwgm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lthtpiov.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3qlxuspsv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sfdryamq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vruozltt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfizfinw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3lodfjequ.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bggiqnfh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3qygshver.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3fzxajjxz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gthhwbhg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3gdobnwxj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3oeyunrlx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xpkyzypv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3tcfjuilk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ifitfmtw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kyvplrvk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3jignomxc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3xgqataqd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsxmegym.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qblidyxa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dekefhwj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bebzxdqt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3awdxcuce.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3hwmintch.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3rqknzdvz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3msfcpyqi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3sxjbkqnt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ymwsdyja.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pwlparha.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xuormawt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3frqazgae.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ikytjjgj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fwqkdxbk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wcbvzace.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ccqvyreo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cyvisqhk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3xvylqasu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rvhtnzga.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hkzqixqz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3scdxeuvu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ugczxwiq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3jwkxxsif.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3fltpwmkq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3pkhntsqz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3kybeovsa.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aowgfdbp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yytgdgsb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3usmarmpv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wdjionts.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3kxcpwwhf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dscrfizv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3odxyumpo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3yemshfip.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nzstmxbi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wjampyqp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3exacioxo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3elaznmxx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eoqtysyd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3owzlemmg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fdyjwlar.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hrjrpqjm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3kjecdtnd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nppkeexj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wyrsswup.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3worszcna.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hutdvoip.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3tsiswnif.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3rgyckmze.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3exlidbhv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3edcyeqek.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rkkrggch.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ndjpgstk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ympdretu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zonkewoh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3diedbtvs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qgelxfiv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xrlzzqtn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3cnaojzlo.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oljkjsex.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3cixavfnj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kiqmsyre.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lyckdnck.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3krhhudor.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qlecljzl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tcvfiuqj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3wgkpypfd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3npghtogi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3lieigcfw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3kvpuoogv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bbnajmmu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jesvujwx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azvqlsws.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mbsozrtu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3sngaeuov.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jrbuixml.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eceoojnm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3thgkiwnt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3mcviywpf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rzxeebli.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3tjyibygn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ozemvtij.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nbcsuenp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jessydcy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3pxqscpll.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3onzystfp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qxitnuyu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3uvoynzwc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3cslybqhq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3hyrkswxt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3xmzznmlg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3myieclmd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3uqiptnwc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3txoqwhgg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3fptmgxck.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3yfhdpxoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wiagmush.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3qiacyqnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ektkonzf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3qwdifuuo.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3aobbfaxa.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3brodsyro.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qpzzqpbr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozroqckk.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgypkazr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3tfweuxyc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3wzhbthav.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hwafvisp.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3zpblcahr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3aucfizta.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjkxzfqj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3whyprkkt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3tzruowac.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgdxpuhp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3agdoexrs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yzhhxceh.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3thhzwljg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3wizjakla.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qrzhbykx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3itajjrsx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ebovpfrw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wstzcusi.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3vfubovst.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3cxyoegij.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3aavjlgmg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3hwceywwc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xmklmcec.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ofhsadmo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvrfoafq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3msrwzfpd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsyrehcn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtmnxxdz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lcceujwr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zidgcsom.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3suzxbskx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3uzymfomv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3jrzgvxwj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cjskjeyb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gkgtnass.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jhqqlbti.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dqbyzipr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3nrobdnll.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ehiaboff.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3mzpfveap.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3kiguyhxu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3jjdparlw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3drrhvyze.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqoayyru.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bnidxagr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zibgpsay.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3hnqimocz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3xobgrpky.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3pkrxomsh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ngdhqwcz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ulhkmcbb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3xwwgmubt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cchhghpr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cfajqrup.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nnbkyrem.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3gavomgdv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3clopuygo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xhivexti.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3bsliance.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3dipuptwr.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbfysscn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mlwiwxqg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3xmzymzfb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3njlovkes.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3vaautqbo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3iupnsjmh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwgvyues.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3tuibkcrq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3hpbbvevp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3dgpgiotk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3bbclcrhg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ucwnsigq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cfzqkjhj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3atiwtizt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3velfcgjb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3pakjyrdi.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3zwpltplq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3swexhqqs.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wqnxvxvl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3htsjvjzc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qpcjkacc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3cwyslwxw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ahceunmc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ucznjavl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3vegwfykz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3balzdill.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3lqagqmqf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qsnyldnq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xcavndea.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3pehcaafk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3altymauo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3luqbqagn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3iwvecstz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3njjkrlee.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ggsebimm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dbptihnw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3exlpbivt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pavtfmdb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvgbqbvl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rwyehyha.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rbhuujhb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vivvzmtj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3afbtlyby.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3voiusfeq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ekfevrjh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hpmzkdkh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yatusfqw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zoglleqb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wqwuvqwf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3kzdohgxu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3uiopihat.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3oenoycwn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3orxxlytb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3bonjyrzf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ogephvuf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3xhcxthza.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3dzqdqerp.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3jmuisiod.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3rjfvrmaf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3btrsxhgr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3umwuuxnu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3rbjluzyg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3sbymgqjz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ikjgekxo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3zlxriwaj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pskkfkte.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ekohwvyw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3mwgubjjh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3vafcwzjz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bxstnfoj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3behcghpk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3gibttbnp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3gruopgll.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kphoblvx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wvlgcqxr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3dqpkrhpd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3uejhvsgm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3larxchty.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3buxodipj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sosorkjz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xwsudvlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hzepzaxw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3momlaivb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ikuoqxef.html


<!-- 参考信息 -->