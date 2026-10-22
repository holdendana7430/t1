代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ogvcuyzb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wabvlbbq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xbzrgzln.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2hhojfqau.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2twmbtzqu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2utiwsabq.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2cnejglxh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2owqvvssx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xlucodyc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lkztmgzd.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lufdpkmo.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2imthjrbu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2aucvojqc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2rurvmnpd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2fqcmywtc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2mrttmclu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2kwoytxjb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqbqwqnv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2npwqiymo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzzolzdp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2uqysrlit.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2yokrkyrt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nccqkdln.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2tzhikiuk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2wwosjzzg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vabnswrt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mqprzqom.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pafuumxv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fdwtdkjw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ewnlmhcd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2muqewsws.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dphtxvwh.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2dxyeawob.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2txnafeup.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iprjwtal.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fmbzyakv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dpwonyvw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nsejslrr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2rifnuztt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wsqmjakn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rbwglsvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fonmferi.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2hsexbnyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqreavks.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wnqaobrh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2dytdgsxn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zjbuolca.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2fuinftzi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2isxvlwyg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bsmyvcto.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2knfcqitv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ptvwjxxg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mhemeegi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ssluhrzu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2imzhnqko.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2zydyqfrd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uertifec.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jiwftvkd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sxbbqbeq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ytqnxazp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2hgshfhuf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2cgeeyrqw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2qlhoxhui.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pkatyryw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vcraxlqe.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gcebyjwm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ntnfsbzg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2tluzxlnu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2gkmvivpz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2egzjmtxi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zifrcmir.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2rrrbpqmd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rijvmptz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2jrbchuwz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2uycfmjju.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kogmixvy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2rszxakjy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2knvjhede.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2sbmqnweb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2sqbzesmz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tzqlpzjf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2wctgoiqt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dkkzfith.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iwzukeeo.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2usfjryhy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gczuphiy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2pqttxwwn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kedlprki.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qpbxkiat.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zhitbdzy.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gllakzaf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oxaujahu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kzrcotxz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cfjsqyhn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qudvaere.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jkqzamqz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjjwhvgq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ohuinbfa.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2sziuchhy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2csvatucs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2eibgqwzp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2rwzytzro.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cpsiuzuh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2jpwwcvzh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2oyustuxe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2daweptzp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2axqywnke.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xtteackk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2bagavgnu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2qvzqwjvc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bodpixfu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2yufqtepk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pzdbxttt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2elsekvrw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2mnpyehwh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2vrygiyth.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2xfixhvnm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qucdwamk.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2petgmays.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ztntavzr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2spueyjwm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qcbwodfc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2karwetgf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kapktuzy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ajkaqakh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ccyklbxk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rzzsoguc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cwfbvxsr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lpnbdljd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jjyhdhdf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2fvswymqo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ohuglogq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cmkiyack.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ncapsozq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2nlxwyaaq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jnnxdfnq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2iwwhukov.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lmoxaaho.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2huhuygnl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2seoexltw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2lyhmlfvc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zvvbmbdo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2kozmffcv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2coxpywsh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2mubpysjw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ohdyoztb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2eygzyfgz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2uprxognh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2qpfqwnbg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zjaxhjsh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2hokntnlh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2glfpwden.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dyzlgqhu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2uqbpnwzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2skmgnbmq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2viijxdsr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ufbsxpqk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ryayypqt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2scxsdhmh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfzufcig.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgkxnsox.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2khwwyxsw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qrcjgalf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2soodhnpb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2mamxpbaz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2oklsvkna.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2dzhxzfmf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2guwuapbf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdoecwpm.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgqmoffl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2xmhcrrgf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2hhmpwamp.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eodszgty.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2nastmjdz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fstsgyck.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2apryocgs.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2obklocvy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2flrwckbf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2pzjiuqdz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2mlxbujdm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2svulwayn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2puudaecl.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2vgdqcrfj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gdvocukl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kemkabat.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tlhgtzxw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkvajdac.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmqjlotx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ycxczpjv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2frdtjncj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2kbocflnv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2vhvxhslb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2nnrmlgks.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dukghoja.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bnbsqqur.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lkkoqktt.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nwtwnwth.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hcxejail.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ptjqxxho.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2drzochvg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2blohhhan.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2urycbakw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnvsssqb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2osxaonpi.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gugvlavr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ccjhiidr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2rottbxyl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xdjonpmz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2zrgebjdt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2mvbidkph.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2bvdwbeyf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gxearedn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tyhvrasf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xipuqxev.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cyiwpaar.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2sgkmvolb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2qlflgbfa.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2yupgssfe.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2pxquoyhj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2xxyrnlsi.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvxtlzbe.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2oblmxlpe.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2pavagepb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2raaerpeq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2hklxykuu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2tfieiogu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2txfipamt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2rmgntwmt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2nmygwvum.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2cvmdpjcw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ihsjtdts.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2hhbpetaa.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2luleqhcm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ghldoppo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2upelrdvw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vyttvamh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2nsqixfsm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2nylgjqoy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2facjxgvg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2wblraasc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2owsyzqfv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2sgjbcnzi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2bfapyjkx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2upjcxfzx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2guwujiap.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ohhekrfm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2zeqxxvld.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ijljkqvf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywmsphiw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpmbhvfo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yamaywtg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2aaaavypr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2aqnhcccs.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2gaxdyvsf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hyxbkgmt.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qglhstnj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2clcdwfjj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bgoekbii.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cmztilln.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hrbenqcx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rleikhxj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zxjwjcha.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gqgamudz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2oomexras.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2dbgueaqk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2unstsxzs.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cjqtbnim.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dxtysxle.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mogseedt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2xpocvibb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ttxrnefj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2vypmrush.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2iylotbce.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pilrgvdd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2fxhsctpa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2bycqtbse.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2muwfbasz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqufltal.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2cqknhgkz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2jheipjei.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2wgjrdjtm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2mrpsruww.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2yoomojvo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lazyonex.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2yrbqhpud.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fxojvskp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2wgfvryrr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2sakfkkmx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2cnmhwtbc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wxmiysbv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2mgmxgosc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2dwidvafc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ewjhwuxt.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2pthnjser.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kulypxql.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2qhhlqjxg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2spqnmhoj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2jzpvcycg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ubvppxuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epygiddh.html


<!-- 参考信息 -->