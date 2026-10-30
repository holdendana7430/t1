代发 wailian999

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/ghrajsyng.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gllyamsgz.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gchmdpmhk.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gifjdbewb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gucpqixaf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gyvdssvma.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gbppkblue.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/ghzgltiqg.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/glhpuvmoh.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gsfhomwdf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gomsehtqq.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gwuvczith.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/giwswkxfr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gpmrisvdo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gjzozfqss.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/ggqlyqvlg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gabzjkwdf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gieszxyff.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gecvwxrbe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gdjaddxet.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gyiyovera.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gjywutaox.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gihaozecp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/ghugfzvkj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gdlegoxcs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gyujtpaju.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/giwfidajv.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gzqsxtmgv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gsswbzsaf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfwycnmai.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gnyftapjg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gltobhgti.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gdocsirvc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/grabloein.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/goryssnci.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gilzrwyui.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/ggquuboae.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gqxjvicrq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gfyawumts.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gllwauofo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gasopixwy.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gvsvuufip.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gbhhfritr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gwbitokmf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gnuqkmofu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gsvgsvhox.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gyntupryi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gcovulrse.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/grmchbfys.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gviiuomrp.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gzdpwzdlt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gmctgufxk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gwxeijseb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/ghsiiwubc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gblqokdef.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gqavzrusn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gagvrhdqm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gijaydwrn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gpupetzrj.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gkicdczpr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gynevkqqx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/glldiiidr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gvgaceekv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gqxtrjcxu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gipoxumdr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gyndhdnyq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gkzxiytoi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/geasspxzk.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gcktjemmk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/glcmkemdf.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gqazcjadw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gpexxtjpn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxhuymtty.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gmwbbklpm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gfarxuaiw.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/glfvaheww.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcgnmcjvd.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gkezxalvp.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/glrvpbljh.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/grzluygwv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjgwzslil.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwpjkxvvr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/grgtrjajq.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvcdqason.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzpshnlxz.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gnztbrfzg.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gzffkirmz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gbklozxxz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gsjtvbqsz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gxapappre.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gfmwfxxdf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gsegvbojj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gewquqbeu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/geybifppr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gmblxvrmg.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gyhjcqhmd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gdcpvwcto.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gwkekqsjt.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gcwvcmpnp.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gclrwnkyw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gopauhtlf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gjyqmukkl.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gbijckoay.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gacjdveda.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gusedelhw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmxlulupt.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/grtjqyndb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gvuczfrxf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gfcghfybj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gpfyafcth.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gmehxysrm.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grtlxjqdu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gdhaiqivr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gxkqrmmtd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gymmbwnvl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gwvqqikqm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gqizotgij.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghonozeyo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gredppaoy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/guogcngma.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcebyjmie.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/glsimkkwt.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gqzqroyiv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsartjqza.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gwxuzlkgg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggdmadfgz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gclvmzboi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gfkphppwq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/giypswwtg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/grisbhvmw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/ghsliqorg.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/ggjzuojbr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gozzpyjwq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gkjcfyste.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gznzyhelf.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gvqygyadb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gverhenft.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gbvfgbwoh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gxyxdbhie.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gqppnpdqr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnkyktsxs.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gmwdpxvsa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gitedrycu.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gqjrdxkso.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gopwugtnd.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gdevhnzri.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gunwuzshu.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gslknokij.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/guiynhhoz.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gfimokaeo.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gsiwzfhqq.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/ggohbjrik.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/guwatcoye.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gvvcjiqby.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnflpuqnu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsxfyxxnc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gadjvntsl.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gaavsmfyf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/ggxfuhyib.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gbabbhbph.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gdomxyvtk.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gzticcbkv.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/grfcebpbp.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/glfbustnm.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gelmmhqhf.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gmglzsbjt.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/grgrfmhlv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gnyxvwpgj.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gpaxigsmd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gxtqqdyuv.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/glpqdpcri.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gfbwdxfzo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gdwzeedvp.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gwribuiko.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gekfjfqay.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/ggshfgdar.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gwhzjhfmk.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gyctafads.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gutirwctz.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gghuoutsd.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gztktinuk.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gffastipq.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/getdhkfro.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gblhpgbkj.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gcgpzqfio.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gmipmmkux.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gvraontjf.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gbxjqhpby.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gfcelgxia.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gmetgcnmg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gvknbauol.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gxixwpqfr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwowpdanf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjjvzqybl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gucrsgwvu.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gydkqffjw.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gwzmgywmw.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/ggyiacqgg.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gazhvcasi.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gcaiuphzp.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gkdhsbxua.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/glbxkzbls.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/goipywchk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/ghsfqvmmo.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gvezstimv.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/grediufgs.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/guobjcmnj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/grmxuhrxq.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gohbwqguh.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gttmrpraj.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gxeuqkbvz.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gmnqimilz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gwtnzhwkh.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gqgmquiea.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gqmjxfkqx.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gblxthuxf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gxhirkfex.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gnnyphxuz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gewmiahrp.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/guwhobtaq.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/ghzmbgxcd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gaikikjis.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/ghdhnptbv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gqfcrldbq.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gidgydovc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gvqrffgnr.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/giqpbfaoy.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gdotarajw.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gpwkntaac.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gygnrvmup.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gdgenqcyo.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gpbpwmnaj.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gnrczjbtd.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gntvxngnw.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/ggjfvgchc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcnmfcdss.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gichgyjpj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gnnizogdk.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/golqkomtp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gmlnpwjlk.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gievmemvo.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/ghliujegw.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gjbmlvbww.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/ggusittfn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gqohxmgrh.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gghqbabya.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtanoodyg.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gdlctdoyv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gwzocblvt.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gdfqvyzyu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gpvmlqjjn.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gglycrjfp.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gdeipuuhq.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gwrgnaxke.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gqfxmfxvo.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gfkwlvuid.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gyjsuthle.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gjjismuaw.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gsfuczbmw.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gccgzqlmm.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gflgahiqf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gcdxdgzct.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gyqyuhrpy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gsmgbtodq.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/grbcffjen.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gtnyuhsoy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gipkctjvu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gjikakbav.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gjulwybrk.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gttvjspjj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gzbglensl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gbctsuaso.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gmjsmoitj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gvvdufwyj.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gmpaudugf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/glaaqmdgl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gjmajlifm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gftyhnaxp.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gahtanrtl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/giurwzgmi.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/grvopcsyg.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/giydgbtyb.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gjlzzewiv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gdxnewvho.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gjgpegbbd.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gbtumicwa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gcgqcnbde.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyjtseyuh.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/geenldlto.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyxrlxunv.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gxgpascau.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gxgfgsqdy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gpyqgrkod.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/glkezmqhs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gcbwdabyw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/ggenixrlm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gmtcpljxd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/glazmeold.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/grxsykdyi.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gvghtwlfk.sHtML


<!-- 参考信息 -->