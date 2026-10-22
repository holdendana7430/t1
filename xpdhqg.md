代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bsoxbwny.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iwssgwds.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wvmgzogv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2sdxqdwjk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2uhxmvijx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2swdvikjq.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wipvbdjm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tivlnoue.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gfkjjjgd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ywjcqqez.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2viekewyr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2smvdekpl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2oftrtpmc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2edpewery.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2wftrbxmg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2avjhdtbm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ucthohef.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2xnqsbrss.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2tcmrzxcb.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2enzcgkxj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxunbrpq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2pukbkxso.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2yukvacih.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2zqqisnee.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2awuznszl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fwhdocuz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2seasxobl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uacreyft.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yyxqaqjc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2uelhuxqf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2apwtqtqt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ugybltgb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2upidpegu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2freubfye.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rtmtllcj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zaenxnxw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ejgaonrp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qifolikj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2jrjmhuki.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dkutkqcy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ljlfkgzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iflviorn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ajuidofp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2npzribon.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2zudywtns.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2cbaucesb.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qovjeqce.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ifcnvsfg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bscoxzwk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ngwjpflx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2gbuauygn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gbbyquei.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2avskazsp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2kurcytvt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2rtcafdut.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvjqjbuo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqyfgyuu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dgtjwjak.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kilmjdjh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xuhchwxy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2glboupff.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2kcrtwkme.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2wcdmjgyh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2nnwbxgot.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tqbjzejr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xszkgjvq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2twwezjcn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2totkqzom.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2jlytbwxn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2odmnrcnl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tpdwkbkx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2xamougoa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2fnatrvhz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2vbaruwca.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2taepsgvb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hijoioiw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nxkulzax.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jovwmscm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2zkwdsmmg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lywtewmp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ygmedzsu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2eprgmkuj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zkzqdxwv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gbxyxvxc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2msnrsird.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mfiqsiwz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2valdqyrf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kzwjxlto.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ndrvsswm.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2saodrjln.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lnjtvtek.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vsoxdejg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ldddnjma.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tvrokxip.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zgrblkoq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eibdiild.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xlhsefli.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kxlqhehj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jdaiykee.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2sduclebw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2prmogimq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qrqwyxdm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rrtdadjf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2hbwsbham.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2zbocvnrr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2mfynhvvl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2rppfachx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ikumufjd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2sbzdzgze.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgwidlsh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hzdsemam.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hymwmdmy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hzkgabdq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mqaoekfy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2axcbbbdo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2crilqanf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2engopqgx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iltkgohe.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mmsxfxcb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hwqoimhw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bkmzuicj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nhukrgiy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2rktbutvg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rdayifzq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2rzecczbu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2uclyxyra.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lfcavvlc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sdybrldm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vjbvzrsh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2auxxmurm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dwvxvmtk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ljjxuuce.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dyuqfave.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ziawknci.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2xuxqidax.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sqrlrusm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rfuubgjh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wkjduzem.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pjbvcoof.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2luojwvix.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2kevqybdu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uatmqerv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2cwpapevy.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2omejthwy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2hxvjdnhh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2jubjoztg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2heywkoxi.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2tlfwreex.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2jvewxulu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2oypusbuz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2lgostbkz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2gqvorrdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkpmfdvq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2kyzxvish.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kuwmzktn.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2sbbukbom.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dtfpirkx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mypndbgx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvmndxsp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohhwjpqn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ymccwuqd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2wlduhkyl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pdhegexl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyfokoin.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2jickcyun.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2cntetast.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggfthclj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvoywihq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2cbvwnkhg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwrxirqw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2aaibapui.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2oaitoaxp.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zcpjiltj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2tduifqnr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ivxhvpwy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2egblybhz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2luhqcpuk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zeggvlpq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2cooizeua.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2malwkjus.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2krohftwp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vjzlfige.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ujsgfssc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2focdixoo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqfzdqfq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tknlonzn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiajogjj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kwfmtmhx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2atfirhla.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2djixklsz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qnukobko.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2dzxjnaew.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2wiihfdgr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2stwiocpy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2djrutymi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjknltiu.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2eprefcdh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2emowntel.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bxubdrkc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkkngpak.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2zthbqtlm.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2iqynexvs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fulyinhl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rvtrxzjm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxtdtcna.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwoxqhwc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2srqodkbl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ykqdvjbd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2kwxkgdjk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2zxezmbme.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xzaceogh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2jvarbaeg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yfeczush.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fitkodom.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pnkhzgsm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2bkqpejjz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ermlkrcc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2lphlakhk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2agczetxv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2stqpatvo.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2abwsiaoe.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xgokcbwh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzfqdysf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2fntegqzn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2uujotnfn.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ggwyazpp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2eczjvbme.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2dprofasz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jamahejk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2kdamuklw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2otdacfaa.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2yqakuzib.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxrrjzks.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2uvezmkrp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2hfuvidlm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cpaucwrp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2egliniqr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2uocojwbt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xhncnhni.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2lsljlago.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2yjtkxqwe.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2bazysccz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2fnzalsdv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jccteqyt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2xfsorseb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ubmgbvry.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2hvvjoaae.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2drdhduvk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixrkqlfr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zmxpyaeh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqpnarcs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jagkzfxz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2izckiznj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwnqdvzh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2umoznxxq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jhkbfokd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eijafdyw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsgiaqvj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yhetbvta.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qebrschh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rkxtirca.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ojrwxjbj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ayrcbtri.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2drdnjptd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2qihocgtl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2aurbcaxx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2goykhins.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qursbwnd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lxjrmdgx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2gfeqctfk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gaixwbuy.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2mgpzktsh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2himoyrqe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2odbacbcx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2fohgpjgq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2fvxtxype.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2hnzqxxsp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmughfhv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2epwvgrms.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2zdvormls.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2fzauhtvy.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2xwqaycei.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vagbwzzs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ylfurhdw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2tojdvmda.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ccmnlipm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2tnqcdfgf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2tnirmwpd.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2tgcvaele.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ebsixrlz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ahrxdqaq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mvvyebpd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2vslyujjv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2gmblpbjb.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2geneblml.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2zrjgqtdv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2fcnbeolz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2tzhgkppv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zkyqlill.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdrlovvb.html


<!-- 参考信息 -->