代发 wailian999

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ewbjjcgm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3tnlqpdbw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3zqrjcixg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ijmjrebx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xeuxjaus.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ljfbqhvl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3anbinbur.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3olgsidog.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3iiwvrbdw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qvplxqhi.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3qnysusub.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ltlwwxxd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3crgculmc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ydsjtovc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3xjjmghyy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3orvyjwwz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ynpwwbfb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3xbkbzizq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3oxdaoxzy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3vobiqjpl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3myndhecd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwoyeymq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnnklojz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gzydjdqb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcyncbir.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3mtpypisz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jymfiarv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ddoowapp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3zotkwhon.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ovkxcfln.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hzcolixe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xvyrtjoj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rnhgsyfu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ikgzbrxm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rbbewbqv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dhqvjxjd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3iwqsunnm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3tfwvkroc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pubpflmo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pbtddjwm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kxrqrvaj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3valvsatb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3acjwoert.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ybeeiabu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lzyqanww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rsufyzjd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3xpjtqznu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqyaildl.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3zjugymod.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3cqgegtev.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vklbvgze.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3qsaonidu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3txynonii.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3damltysb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3pthundgk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vqnrcwak.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ebzatcfp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3juzspzpe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3tjbeokeq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3cojjcwap.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3thniokpx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ytdxsvyg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kkkzlthl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3nsnpkwnx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3anysmehv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3jujncmey.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3niujcxsr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3boayobge.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3smpehxuy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xemxsbtl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rkwthxpi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ahezdvid.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3huhqgdit.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hinwitdo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zddktmyg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3dfwnbrdr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xjupevyy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3rheozzij.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kagsbhei.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3pkdrxfqy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ttzdnyei.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uleakqqq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3jmoonddg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hcbzqcld.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3yvqjgkwr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3cleswewi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3brypnjdj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3liaagbrs.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kydqlckk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eoclspue.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3iyknplys.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fxazyhdr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ymvuhkth.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3zdgwcfpv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uxbfihtv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ifpuokmk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3neroabtk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3efhfjbos.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3krghywtr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fgijgcsg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yaibhwll.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tzphhcqd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xtgbkbkl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kkyizhea.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kqfzswob.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3uwryaifx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3szapxjon.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3nkgmrlqa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3yujwnufi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qlfvpqdy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3cshvueza.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3hytsrbmj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ckxfhesu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3njwdrzgr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ayvtpwfs.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ifznsgts.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3gezcdwau.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3smgoqnnt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3rruqfypn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oatlteer.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3bveqcqll.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cgnorzdb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wpgcnzgw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zybpcsdv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xtqnpddf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mwlhuimr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3iwcwneka.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sllplcvf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3eexzqrao.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3zyozwepm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sehvqyng.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gvygvkqz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oinsxkjt.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kyyrylkw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3hxvsnmhn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sdvgkjby.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rlbejsba.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fbycfjqv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3yppqokyc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3njcpahhy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ccraqkxk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3edsingjc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jnmzdtqx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rzdfnvhu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3suunnzju.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jykbuasb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3zwumxhcq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3urwgqqzk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3eaazylah.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xuusbctf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mrseylat.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3eisqrifh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ljhtqssx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3mbkusofm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3msnvgyzw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ultyfmhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sxifrdgz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ktbsmssx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zgtjobga.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3dsluxliy.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3rwvgybfi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3itwoondz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxfxavba.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttmedkqc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3paaqetvj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3pwyulucs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zmjmdxio.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqvwryxs.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3kiqqspqc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3yjvbknfo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kuiytqsq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsyydevx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekdwrcpn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfutypwj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3nbayxdpp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3lwvvhhkk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rrsiflch.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ildumoax.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3npjlkqsf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jfmbowxl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lfkllhhi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nclrvpub.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3gksoptfr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3bpqffofv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qesdlpit.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3uboheizf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3lulgksmm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yuuqnoph.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ftrljaau.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3faxquaxe.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3czdjufoo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ltibtxvw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jxqpvghi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xnhcykst.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xbmmnxyb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3yoajpsbz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3fexihahr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mytcokxn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzwxsdft.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jjfpmbrd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3oeidlfhf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qzqackbk.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3bgzotyme.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmrgesge.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3jaganocr.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3cvqjbuyq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jrwttepf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdnypmkq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcyzzmqb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggsnynvy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3nowpepng.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3akbjetak.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3mhjcouvh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3knpldlpt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3kogjyjxy.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xopjycqj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3evejushs.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nbttlooh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aufbrrpo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3hkewlpnh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vtozumhl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xmjxfzdl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3vmslqfxo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3fyoddemj.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3isrrwbfn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qltmhjfb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3afchmxpm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3snbvilli.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3rttjxvhm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3asrfblwf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ilbzdbsq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3iczpeath.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3zjmopsju.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfxpvvsw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3btlmtjne.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbvabmsk.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3dcwbwwkf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ndnekesr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3skdtdawp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxvhkpff.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ultgkdqm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3wmezbjns.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xbxgkwfs.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3nloszrby.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xfjxiyyb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3sfwqwmwt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3kpzdnzhi.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3szhpeilm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3miozrafr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3rthgjncd.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3nlhhqpyr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ebawlwgt.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3duuwwbyc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijbjuwdm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuilorms.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wbpxpuof.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3mleddday.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyilrshp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3hymbucdc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ppqbrdjk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qyjdswjm.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ysixsubq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xckmdejt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ejarjzga.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mfuhemui.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hzqsmmfl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ysvriwhi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3yvgjdpvk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3nllzumgb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dbvzaoow.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dcvyyfpf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wbjqzsgv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hrmvcktg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3tvkpfplz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3vreutyqy.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3xcnjrjas.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ntefnlmu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wirgctdl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3pmkprvke.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3esecsdzs.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3vsqoiavk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3fwsziddo.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3byiipkcr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3hcohahjm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3tkoscsqq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3wxfakuyg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3iiusmdyj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3bzuwvfuk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3hblmdarw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qlaxqhwa.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3kjtrhcvj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3pwpetkap.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3watvzaky.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3khtanlqi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3bydfmchu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3sujggjdl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ottzsmlh.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ebmzroze.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vcivjebt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3dliwzbxv.html


<!-- 参考信息 -->