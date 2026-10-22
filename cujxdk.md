代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2nvhynwqn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2uvifipfw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2xmowxroi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jhowkrbv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vyydblhm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2csqoydid.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ywxtmpob.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jasjjrur.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2bcmoftny.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2rkztyufk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2iboetbph.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2sdpgadpx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ddpjjknx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hgfxcdlk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wxrzsomg.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2viujarnw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jkftpizn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2edaeiplb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2bbuhwoxr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2horziqcv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ezfrtdtf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fbnffrzu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nhxbxipt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ctgyekgp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dgeardby.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2fdmfhaiq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mwmwiiyb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hazftlnt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2bogalqci.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2pyvyvtzi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qtpprhhb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wfvyoaoo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2omnzaast.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gchwygyy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ltzzgkuq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cparuyqn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2derywflf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sxtohmlw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2bhbmqspg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hgwhlijl.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2jqrcayyg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ocnxuycc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cpvwofhy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2zheigfyq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hmolyqeb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2erjatovv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2klnqzyjv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tshfhkdg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ojcafdxi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2brkbqeku.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2tzwecbdi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ytdzqhvf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kbpqeioq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebwotbde.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vdhcfchz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2fxuphdux.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2nkkntvtp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2yyaqdgjt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2qqalkvxz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2azrqyxfy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wapbbetk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2frglfjnl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jfjhqyms.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bzxumyai.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2fpvlichh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2irsqxetu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2cvogidef.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2etjywmvq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qlqvxhwq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2cjlxhgxr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vanmfjso.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xtnwytqx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2midnjzzw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ddsjdjih.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2qmmmtoum.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hmxbuuor.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ggqlcejw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2bijgqzms.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bhmmyehz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vhnxjtqo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kudioeuh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kikdybkn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2bruobgyo.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ddvsjovw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fpexlrck.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2rkfsxgxe.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zlgaqelp.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pcwuvrpw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mkfdsdfv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ciyehczz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jpgczheg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vgcsbwkz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2edmxjgns.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2msokayjb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2hxxznvnw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nlwilhlz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2iorhljnk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2klwpxyzr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2oynvbmhc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2jwkzyhiz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2reoswaal.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2etzjmjkg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zsxzolic.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ytawrkza.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fmwwpqxl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2daqeadim.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dqcqyxzb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zgctubgy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dmvgtmpc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xefevdzt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2grnnhubr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2xrldoikf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2epgtvotv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2akakolan.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mnhmhfuq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2izepliyb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zqnljjda.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xysxrdft.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2vwvmzeoa.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fwqojftl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2aimkvvun.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2zyxzgqfe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mlnfwdzr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xlrglntr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hljoouxu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmuxlzqj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2nkvpmhul.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajwnusrj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nxhfdndl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zjhvopan.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2aogbcjbg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zpxbnpku.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2lfrisajz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nsiqqqum.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oaszkcer.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tedcogoj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2puwdpngh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ectyfuau.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2msghyick.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2aavygqrr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2trndnyuu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2fbteuwky.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2elqonnaj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2njguditk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2kjgfgslr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2yvxsbkww.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2rtpnfzqh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2tfapsjkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukvwzfxn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2mqitxylk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwxahlgc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2tswwkoxd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2dnbxizwl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2atkcfrfx.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cohtgmnt.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2qvlwftan.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2slqkqyhc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2rvbyrfij.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ysahnogl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnwwmuli.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ojlmqlmk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2hjxtafer.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgysjoip.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2porimfjq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2uqaqmohm.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2inirkliv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ojhosruu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cghrbfga.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xeevaaed.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rlqkauxe.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xaqkpkrw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2hyvchdfq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ywpewvpy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cwdisbdd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2kgxfycoy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2mgbgrfjw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2shibkcmh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2oxbqgdhh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2xsyuanwq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ccxoelak.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2olxlkkoh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rcbadeay.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qyznjxeg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpjbnptr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mexghtvt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mhfualgl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2oadctwmu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2pgtlzjck.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ciugyfqx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2syrosyto.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jmbjstpq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2snweckty.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2trymwgpj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2gifuovra.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2osupvena.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rkwmeycm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2dkwcyrzt.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ateziltl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yhqfaoaq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mnhqwbks.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nmkxedva.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2coxkxdxz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ogdwzwoi.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2vuhmabth.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2tydhszfk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2hedmtwjs.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xdkafplk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ndobfyzi.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wgjqydwp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yoylibmp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2supjqdno.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2kngdfksi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2asivsjoa.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mhmlmlag.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2fhgzlfka.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2kedxvkxn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ojrynhwu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkhnlgnv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ivicwrpa.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2frighqlx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2tixayytp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2dauumuqo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2wdkqkcqi.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2nmkophaa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2mjulsjrz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2acrwtadi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2werbuvaf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2hijlkuas.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2hakgdwwv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2pxpnjeyq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2cexxhubu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2gfnetquo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2olhohiyb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2piqsqyfp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hgkhfyax.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2lrvnsjpy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hbcajtvj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2inxuqezf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2fxqljowe.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qfitzahi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2sfsjacls.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2szbqmouw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2hfymlgoq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hillxtux.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2usjzxckk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rhrhcpfe.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbzyrhhp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fmrcjvli.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2yegqcddf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2nezhgagd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2pxkjnqpl.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zevkbwyp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsbukjgw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdwgpror.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mfhwoetz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zysrmrxg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uiqinrjq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zjdubpof.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rmiaugpf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2dghzjgim.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2poxdgqqe.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vbfbdnqv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fpxerion.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2shuegjsd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2webcszzs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2vewjykgn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ucysqyak.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2mgmoppyc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2pqecggzl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2oxtlqqwr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2hukojaez.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2nueehdkf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2sexppmts.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2bimplffp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2qtoyfler.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2aighjdcu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2miubwihc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2oyyqlias.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lkxxchrl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2cywyqacr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2rukbixky.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sbvkmzfi.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2owkqisnj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2meqbkuod.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2mnqdfxfm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fivwqdaj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2klgxcgrv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2tmjjnmdu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2vcubwuca.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ztlcndwo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2poglzpml.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jpcfpyrv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2bjxdoqhl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2bjutmhjv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2krdfskjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxmomiwt.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xoplckhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ykrfnfas.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2pgfkqnzq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2izpwfgap.html


<!-- 参考信息 -->