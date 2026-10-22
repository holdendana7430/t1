代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2hmnaumqr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2oanjwskc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wnviovcr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fhvhthyc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ikrkbxcx.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2adogoqst.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2rkbgrztn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2oowdhmni.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2gwdjamqw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2tugzpatt.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2likbgctc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2byyacnko.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2dzgqkpne.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2hilcaxet.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwyqohfr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vjmwhajf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2jwkofbek.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2xrjjgxkq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ctaptbfn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2imxpyehu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ulqugnlk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2npqycdgl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gmlhyvtn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mzekefpm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jxpksfin.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2kjpltiws.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sclwxhme.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2eatkdcwu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2dwtoakie.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2bjegezhr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2atwkverb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gganmrrt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iyucvftp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lnzhfuhy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2grnkmqtt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yhqqvfqy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2exlpauet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkoptiub.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2qursdcip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnetlzov.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2slibbrix.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2xxoytnqt.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sjunfjpp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2vwetvzqi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2owfmpxbj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2llpuwmwb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2nfojiygr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pebacqjf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pidmzkhs.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2yqeakwhj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2kpaakrgw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2soprdgyx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2axykdukh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwgcljce.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hqgrqywo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2csvrklsh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ucqlmzek.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrpzrbpi.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2zchljrfx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rsklptfz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mffsenzh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nbekesrt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xnejlvvg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2qptscubb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2tvqgxioc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ddagjway.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hbcmauzr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2cddalgvz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sutoozmf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2bvgssxzb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vwrcxxdh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xwnbvhna.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ubnakxfg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hfrjmmnl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2yhcjqtaq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ttpkeiwn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2sjounvnu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2vojxwzrv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zbhhciom.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2euocqdfb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2noylavpi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hvavbudm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2kpfzwkbx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qykndyoa.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bpnbdzwh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2haegssfg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pqhtknab.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qwvxovzq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mzwckwxg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yeuatnpf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bkvsrayf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xxlupkxh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hppbbfql.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nqexiife.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2wpynwzla.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ypxxsugk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2olshuecl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hrwcpetd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ywcayeyu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2aiqvjeey.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ghspsfmc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2cypgcxbk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zxugvvui.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2tglaexpf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2nlbospwc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynvsfwhl.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ckffchsr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rzpfwncv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xwoxvsie.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2fesehzye.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qtmvuvty.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oacyxxtf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ifimllas.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ttztgfpp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sthtlfdf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jonqmamq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rturlrni.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hkoawhja.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2wnotbjgc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mxhqarti.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2wcjfctmg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2vhoyhbit.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2blwvjjyd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jnuxjqua.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zmorgeyv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pprynouz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2njibdnkm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rbpfybmu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fnwmeyra.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hwbqyglw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2vimpazia.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rfxuzbvg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2gqbtnojv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oprwfjin.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2puzcytik.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ufbonard.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2adpunjdy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pqlgparl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2qrqkzugm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2exdxsdsx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2vqigmvjz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2hlgaoyat.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2bspgjjfw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jekpzpfg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2sdiunkpi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2qzevsxmo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2aumsggpt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2mylcuuqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyxovhse.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2jrgmtexh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ninmeksy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2mvnpkgrd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2apwbecqm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2menlpzyg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dcafboqi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2fczsokpt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmboxgfp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2kirsgvea.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2lfzvtriy.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjdvizbh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qembdvxc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2sayyqcgg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2zlbflxbt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdrbhvlb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlzazsmv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pqrwtqjz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2npfoducg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2inzxjluu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2axqhivww.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2rbimjbzv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2oedjvfye.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mbprbvkj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pjpxcgho.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2flbdwtjb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ahkpenga.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2vyteiine.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ryaovfuf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ktwiyzcm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ecbswvzq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lwoasxaq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjnrbtib.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gbxjsvaz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ggwvxoxe.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnrekzcm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ywaajzwc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jqbvqbsv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2aublpznf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2vbhtsvxp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2pbkjjbxo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kggppmrn.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wpgvewrh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rwtsflta.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnuvupth.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2mngfftxj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hzodxcws.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2arxiodxv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2fmddgsgg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2mrxjrkzc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ffsjeqat.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2evlhzxwq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2msndorof.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tnrebqht.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2aitljtpx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2yqkgjjmv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2gcbbxmed.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2qjlsrnvn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2nuentmwu.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2llcedtlw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hlkrrmtf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bkzfrhgv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ghmexags.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2pbjknszd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ppbfzdso.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lrelynbc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2rvczxlqs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2btzqmhvw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2nkwiqjii.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xawbjirk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2nbcgesnt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwlmlemm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ligaszrs.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2bfsbvlwq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpnhtokm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2gyhwxkeo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2kxpgpvgm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2cuwgzbil.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2exclnwtd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzzznhpl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2oisiqbpw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2tqhuamrd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2suhacvyg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdbtjhkt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2qmmnjaih.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2rbyhltht.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tsajalul.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2abgyqlct.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qaztghmf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2tacbifvt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2zqbhqlcf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cdfpiqny.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2dgovofts.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2dixqbkks.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ifltqaqf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wagoklew.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnkdrxvy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpvfdyqc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgsxones.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qnwgvvtc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2yvhveqoe.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2afjvlnha.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hykgnuqj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2dkbpphdj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jvwnucbt.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ahazwcvk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rebfeigz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2spjxurbx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yaqawaiv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mqfjyopa.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qtynshvr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fvaamgla.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2eqmukpvj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pxijnkwu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2joqccmht.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iheyjfbm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2npjxkzzp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2knfexdfd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ldsvfhjz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2jdrqmefa.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ykgvgskm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2sdxafnto.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2regcymsj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2fphcpzth.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2vghsefri.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipbkgzok.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2jkmrrmch.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2mhvfygro.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2nfupzoyn.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2bqxcbjik.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lcczithr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2sopmppap.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2zpqurver.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mlxhhqkv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2bwwkegjj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2wsdciixz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2nvpusyjs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ulrvkofp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ojfzbqdu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mnffyqui.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2qmqyrddk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ibvrbjbt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kyekoanj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2vyrgnxwg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2stoiavrp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xfduxhxu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gurobolu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmyvwtnf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2fhpqmovt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2legrzwef.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2zrtkadpz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2butvlvsy.html


<!-- 参考信息 -->