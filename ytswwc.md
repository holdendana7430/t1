代发 wailian999

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3oggpibiy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3kcetmkce.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3jzzbkusi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wiohwact.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wyhkcncd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tigkiirh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ekqmgzyr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ugeiuqqp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3shzycmhf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3njrcucst.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3veoagfpn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mvdifuol.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3aowggkqr.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hrccfpkl.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hxhcjfzk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tganvlvm.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vyelarwx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3vrdojney.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3xdeitwwo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3soemzfpc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rvqpcczd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bajwomal.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3wylbrsfm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3aprdkuke.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3urvunipg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3vyllbgjl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcwmvcsm.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3mgusslln.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3klolhwnd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rztqfthx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hwxhkvlr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3twiurqdn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yzhpzxyy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3rjgbhwap.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3codulezt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3segstzaf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3uvtcbpdu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ofdxvrbu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hoebzuma.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jnmflccg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mlkopphs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3etwkefbx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3aqgyaxcg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wckdvqmi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3dsnbyrtl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfccejgp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3lyslcyhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ysuspgzl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3arhfxitj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3moxgeqlf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3drdrvmld.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3mjimmqgv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vvbgbojf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ywbtfsxi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3eynegdlb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtukdvxc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3exsdjrbd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3wgaylgdl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3yegwwlxn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3elrscqjq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjrcpqig.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3itfuximt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3owjcrklv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3rfzpjzxh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3xbiibbbr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3axdhkvps.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3hnvkjhrt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3dsujrhps.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xnmavita.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hsssovsk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bmjgskqs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zvggreqi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3mxylwbnd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3pjdhnozs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vlslnldx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3tkcevbnf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xoybdpuz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3tplzkwde.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3iizwzawr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xykbhdof.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3xerngzwd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wsrdzzdk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3rmnmuglp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ztmqsatp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vkzdyirc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xrdmgcut.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rscnuyiw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jiayvdix.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jruaolzn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kkzsiqgb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3huloddzk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3emanoptz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yrnqpxgu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3sbmvuuex.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cbjdpfoe.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bkaeydfh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aeesbnbb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vuurnnmb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ovrbgrqw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wusmjocm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mkpybkto.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hshpkzvy.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ycmudlqs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xwegkkra.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3xmjndxth.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rwankbmx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fqamogjt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3fczltavz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3zhgisxwh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3nikzesth.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3qnzvwsxp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3pmaubowf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3dpwcwazk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3jujwtzcc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ctykiect.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wmhufeyy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3njnbjjlp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3orfxocke.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lkzknzdc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3hnjloxvq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3oewqltyx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hljqtnhn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kkonqjke.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dujqsdlc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wmbqcdng.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3perxejjb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3bbemajhv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rfmpwicx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3rwxojooo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3adhjyujh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pmqebwtl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ifsbtnpb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3spubrssc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ctikwudc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3uofqkhyi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uryyjdos.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gumduilw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3afdrpkoz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3kikkkqkl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gormfobf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3euayxitm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ykftnqpg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sqqpkrxg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lhbjsywb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3dgzshtlf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zkoiyqje.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3foqlxoyq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3sjmbesnj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3mrlyeknz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3inzdjmqc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3stquyvbd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cbgjhjek.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3xhmrwemj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ucmdlcme.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3qmgufbqj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3avitcbxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hjvqrlmh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3wepntygq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crzyywdr.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ymwanpqs.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3hxoodcai.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3pgycuydi.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3aszwyuku.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcnoxdtq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwqsnjoq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3zvixptpv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mwcqdkmd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yexpnomg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3bxnnbxtg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3juenartp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ajfkjvko.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3muziuudh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpmbrzvb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rqraquou.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3myvqxgky.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bbefiocu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aktjnxzf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3kbfgqwke.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3paaxsqhv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bmcdrvso.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jkybbshz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gkjzbzeo.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3rzbbxymp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3syajraxk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gpljhezr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3zqhkwayi.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3jaunzijy.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qhskuffm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3agmwhtki.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dlgvwiig.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jelknkqd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3idyvqrhy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3recwsjna.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fazwmndp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rkiyiedk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3aybicaec.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3rslnzdut.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrzueyft.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uepcwxec.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3skhnhlxq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3imjsnrrx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3mexdzxbr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3kvmjdyti.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3hrjhfbff.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3lhnvxajo.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3tjemckcc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bojxfwov.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dofakzbz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vkuijaqa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gxtwvwad.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3bilpfjyh.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3nydkkxhc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3buclotib.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3aifpbkrx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3qwsvedqo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uhoertlj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hlmydkhu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zptpdxue.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bbzkoaqe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3dnszjxnn.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3jpuyrnyl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sacvbwsl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3rrzxsmku.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3fczqduwp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tryeekcu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqrxyniq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3qkaybliw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3mkirkzyx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3dqgsuqrz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hlrurpem.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmcmhymg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3fcgyzzgr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ndoikyxh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3xujdlglo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gugaljbo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3hrutekpy.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3axrgiora.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3zhjuzsxo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3lwspyxlp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3teyycxop.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3mzgqxmho.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3vlsbnvcl.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bttfyjrz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3umkbvnnc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3anshnvma.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3iohzryvq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3mutvaywl.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3evcvnsrm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3lhfrqsiu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3qhguetmr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3nlpzqqmm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuntzppn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdmejmgy.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ysmdlzoq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dnjshuvk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gkiarzoa.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3pvvkktja.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrvdyktc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jbxsomji.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dbpuncve.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cagmhvpd.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gnwiuigq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kpkezogt.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlsicmlj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vsgeypyg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fybxrvli.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3sqtqfjdk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3kkasfxdg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3rxwezmwu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dbytefpv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vjseiejh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wcurizqv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wozdatwl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3otdtfrwn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ndujeiuu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3xsxpqsyo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3fkkyfdqv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3cfbhpnwd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3pghjojbo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ubmxdcoe.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3gxctclel.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tuzhzdlr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3mrfrmoks.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3beeyiviz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3zdfpgtbr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nbxzwxlu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3iwlptamp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojympnux.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3enshdvrm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fhmbgdzp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3sxkaorbz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3jecfavix.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3opldccpq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3dwywhypj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3zfcyqall.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3iexpngzg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3qzjkjgij.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rplygeix.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wqyafrir.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3swbnrdmf.html


<!-- 参考信息 -->