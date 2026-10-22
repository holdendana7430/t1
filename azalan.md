代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cdcndxnm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fuqjchvg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tweavydt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ofdvkrgb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fgudmixx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ujmwzlbx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ryfzsaip.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qeifeizj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wcwfcnzu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vvesodmk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2czhbmyae.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2hqboaqzx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2juubkvvp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2igpwzrfp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jowvwstb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2imgedygr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2sjjvhqfq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2vrtjajis.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2erfnicwh.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyohgjxs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2entqesca.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2kghvtkxs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvuabksv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2lbqjheup.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2spoulplo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eifwgqzm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2npwckdue.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fymbuqnd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ewwnhhgg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zidgylvv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hymiaotc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tqadbrey.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2kbvrbzuz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dhqvesfd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ybxthtpq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qwimebns.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2grbgprmz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2parcjitu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2qrbfedxr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2toeobtpa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tzoewjdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kcpggskc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2sohthlln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adpgcaxf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2nsmmmwyn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2qcebthkc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fncofgnx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2nzledavp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ltlmotod.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bdpgdisy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2jmfvfzou.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2avtwmqwj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cazwqpat.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2suldfjsw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2vhitanzo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2miqinxui.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2peypobul.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iasqgrnr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vxchijqn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2bwnuwqnb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2mfzoolyg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2vyguvuxb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2xvtrzqwf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ljgwvqns.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2sznrgwnq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ivbkugql.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dpvmitxz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qegfahrd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2rvhwdovd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lvzcuhjg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2grbweyhe.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2layhktar.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2dvfdsseg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2fejcqtcm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2esxmgqmy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2syglcdqr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2iprkwguk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2odoaqpun.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2yahhjfmn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2cvhwbjnq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2twzbxpal.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2spicnuve.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hiufilyr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ivajvwnu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xxdrnomb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pglcdmxw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2fkcijayd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ovjxnzoh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vytfqkgm.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2zlrcxfpb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ahqymvdy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2krfuklxb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oroumbls.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhcnkhkv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ojzcqwyx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mzizjsvg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mqfzulqi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2crpaljyp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ptklkktd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2btasfmyd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zvhoepyv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2blbojnqj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zrvdmark.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2fyyetqlv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2sztxksnv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2wphgttcf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zpkdfuhx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2aggunphf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mzsxpcgq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkglpiuq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bclxmuer.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tmaqvsmw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qzdecjrt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ygxgafvb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2cwbmtjft.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sbvghwfj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2caaygpbw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lkjfindn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aqkaiukp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ceeydioy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2eqhuyggj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ncucyidd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2yuefmynn.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sdgfbblr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2bxopdjdk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2gjoxxddk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gddizkye.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wyvotbpd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vvjtjzty.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2plkoauuv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2akcwxwre.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oyifpkgf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2acqxirom.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qlnsiwec.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2obwabvdo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ywixrwbv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rfwunvxl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bqcegswm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2acvjdmzm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pghbdsyf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2onltudjl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jqpzbjgy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2tdbjstsj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2xwilceyt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2tbzlqsxm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2xdotmtcq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2repcnrzx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2iwynnaso.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2rwyovrxo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2agimloel.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2hxjuezzr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2nnsrvnva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrxgnjdm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2xbfuyhhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmlgelbx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2tiyqctji.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ujnlkile.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ouushlbt.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ziqnwymg.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2rddxzzbj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmmsylaj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2midtgpof.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2jzjqwdud.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rxygenhq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2onopzctg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2wyjmfkdp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdtniecc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nuzikzke.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhaqoyqa.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hrptbkkj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2iselsewi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2urmmbvie.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxplcbqj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2atrzrykp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2znarinei.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ldbyxafz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2sqpennvk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bgaudwho.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2meenmcmp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2xspuhpos.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2drprxzwk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nazxyiwb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2bmktkikx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2eesrakem.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljikuwiv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2czvcxxzc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pbfenhsk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpngfcal.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kfzgbazt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hihyyqor.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2olqotcge.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2wzgeqfrz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2cvviknao.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qczsetvq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fnlicuma.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ttglrjdp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jinzzzlo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2flizvbil.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ddwdhxzb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2wadnzauj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2erriwwab.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2dokcjazl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xpzawizs.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bvereccy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2spvsovsk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2clypajyc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2iylgnjav.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2fjhhfhvt.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2lhufiwyk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2zgbbwlty.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2uzbmyvyg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2qfphlead.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zqfkgbgu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ejgamibm.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vmydjatz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hivjdaae.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2chvhapnd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2drvwmqxi.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xgspclir.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2pagoatwc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wsirldef.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2twtjdhko.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2idujbisr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2igfhlcmv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2iuiatjab.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2aqffasoo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2acmiyojh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2qwywquvj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2xptdhgzp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsmizjur.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2yyptjqwb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkuerksa.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxmbazyi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2lnezjhqp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2lajhrupb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2fajzecgx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2aehjeiwf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2kbrjlofx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hfdifude.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2gabhbzok.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kgvyrpcw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2zmrydzcy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2oedyzmsq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cfwjprdr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2tjtytzxz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2mkrejwji.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2horrtdck.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xstpekht.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcfaauyn.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbapckzw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2milqltnf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bxnfblag.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2xltpigxs.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlrvpkmr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oedywdqj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fscrvqup.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghxoiwjl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hjmceswb.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hvcilppg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rgvlbwvw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tugdprak.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hnbshocl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xtufsbbg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2dlonlvjd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2fhzwdtzr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wqbuhonu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kqznkrnu.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pambxyjx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fslwqucl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zjovjslh.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2vitaimfx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2uytdnrzo.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2spwwwltk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2imhuvumb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2xgojetzf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2undfbsao.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2vjyionkg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uyinucng.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2pwdbhdiq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ohzogkxp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2bspqobch.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2awjwqzjd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2uaaoofuk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2msanzfmd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2otvfjqik.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2lwsnbbkx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2dnvkrphu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2kqcwyvid.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2zzmtlhry.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jzonxfcb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2gebzauvt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2qdhcipvx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2tbmhczcg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cgvkqqof.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2juykgmqo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2zumivrxi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2tmirxhmh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2bbbzqpsb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2uzzgmtqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmdjpsow.html


<!-- 参考信息 -->