代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gnushofwj.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/giqjpapqk.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gecdthdmh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gaxljaylz.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gdkfspiat.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/ghkixjuol.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkqzlnhww.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gmvivgtnv.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/ghipyfuni.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/glasvxprp.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gjjqzeuyr.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gauabfcwt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gmvmpexbq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gkqrephpp.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/goiilvmju.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gvejsygsz.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/goqldksdj.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gcylwtrtg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gcypnfxbx.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gprzsarht.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gfzkscdhm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gyfzbwlcw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gowqrqfcz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/glxfioihh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gwjkdmxrv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gskknbhzx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gllbvsjej.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gfxxkgjip.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gvcdgebuf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkqzzyiae.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/ghyyyoeqy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gurjsjihs.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/ghaarrppv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/guoteyawr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/ghdimkbua.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gxyeqxctx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gkyxmysjk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbfiflilx.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/ggezodelz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfvdaoffj.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gatsbzzau.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gadenysbp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gneetldzw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gwjwykjnw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/ggchvgqig.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gscrkuonn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gsppectcp.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnhgglbuj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gpjzwclli.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gvrliusxx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gwisbjifb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gwxkbmgtq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gsxcvvjyf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gaxlyodpu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/govegsdud.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gmvkgkcxl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gicwkbkhp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gqertmjpn.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/giujpyobg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gfvtvoomr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/ggbthkwfq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/grqtdzxyq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gbphkafzu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gfijunzha.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gablymkmn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gtfkxciqp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gzurwkwtt.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gbozjskow.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gwqrsexfw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gqsdgpvkw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gweisbogu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gzjiyxhqu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gfwgeikbc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gzvunrrus.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/ghzdutavk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gmiuzelor.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gnbiftfsi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gzmbqqjsc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gwhitbzli.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzwojbgpf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwmelvcrm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gjnekxffn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gzhwrqbia.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwydmyakh.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gexmlipvp.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gbzgdapby.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxurfdkrw.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gkmwwmtok.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmbbqjxtw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gljvourwz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gpwnrffnn.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/glzyzmjfo.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkvxujili.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/ghweuguny.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gyagiaybx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/glrlshuuo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gzudlauko.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gecfukfqn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/glffdxnpm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gqeuhniqp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gnlgbrnax.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gwnjbhrgo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/ghpyiyzya.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gqeegktwj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gyyiftcqw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gzlxzwoil.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gslenyneb.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gvyvwyopv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gwefasshu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gwypsfhcy.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gyiucvqbm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/ggxawlbem.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/ghlufyvxt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gooxgjzns.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ggrgdldrw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gtjfsemvx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/glsbwclhe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/grghrrtlu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gzfomzzbn.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcfasdoiu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gfhgivohv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/greeviohw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gveyomgyb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gtdrvuzdp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwohqjijo.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxorvlzrj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gclvfcxgz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkmcjljez.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbptqfiik.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmasznmcb.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/grxwptmhu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtsqctuwc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gthxanodb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqwtgwlaw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gyocfxgyg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gkezubusk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gktlmujez.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gkxpiwtrm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gszkwvpkd.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gckeycwny.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gpoaxucim.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/ghlftznfv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gcidgujfj.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/glgyvemhf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gfifxuitk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/glrbxflej.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gpawnyztt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gjxquefaf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjkyvgikb.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gkwzjtlkn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gewdhnpke.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gnwofftuz.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/ghywrgenc.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gswfnmrfu.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gxgakvjrb.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/genxxylsv.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gdtkeogtj.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/grwdpsywa.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/grzpxaany.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/grdelyplm.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gwnetbvjv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/ggsmghktc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/geablmvtl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gjzszalxp.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/grofbrauz.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glerlveox.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gavchvtck.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gqsyxgsbn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gekpnxaxz.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/glkbuynbm.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gjugkmyvt.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/grojgssca.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/ggovbmqbg.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/getcrcexk.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gyfusjxzw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gtrpsclkm.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/grutlyqtx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/guiayyfry.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gsfbuqqwr.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gnwubngqv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gztwsbdyb.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/giznaboiu.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/ginfieqhl.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnigxzxdt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/getkhhkex.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gkbszpwer.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gjrgxmjol.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/guxoneymj.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gsukvnypk.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gvlvqvjaz.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gvpfccxqf.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gjbekeohr.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gdzdeuhog.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gciryuccp.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gcqvfbkiq.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gxtzmtwcg.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gplfjuyzw.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gpggwduqi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gwvpiooba.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gnvzqfmzk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gevwbxepu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gaulxjgjr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gmlewzemv.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gqdedkknf.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gqtcdtavq.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gnyovmjzx.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gjvsawcwr.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gvmhcpgdj.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gbyudjlge.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gdznvoajj.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/grlobfrwg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gjiaeprhj.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gvocqssdc.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gcwwxsird.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gwqjqowad.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/glovfwegh.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gacfpyxlb.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gzyghssuk.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/glbzjlchi.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gipujowwz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gqtimxeuf.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gkkmovwjn.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/ghyitggve.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gozohkfnx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gcwquqxed.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gcinsyble.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gpukddqbb.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gecfptxxx.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gzcfyixbo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/ghfxwbomj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gglvroedm.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gpqjdnhjy.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gilxlhorm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gpmmpwvvo.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gcfxchhtw.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gszjmsdgp.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gohtunbzu.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gqatiiqgy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gshhpvfnq.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/glwjnsgpr.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gqyggvzio.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gqotkstno.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/glxjgqtbk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gtcvcrqky.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gstpmujol.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gifnlxmeq.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gqusethkc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gcmjvsncg.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gssxgxoum.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/ggfczdjes.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gpxoddxhn.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gbekcejsl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gwyysjaaf.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gswraustg.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/ggqmdvxsr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkgwabtfz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gghxjgkjh.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gsrplteyn.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gmjbfymjz.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/glpesjyfr.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/grslfywwt.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gxnpwqbss.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gbrhpjuzy.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gydxrdfso.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gaprmrnia.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gnbmhgtww.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gimizaycr.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gbuvifcpi.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/guhxaqceb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/gniwxcumh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gkhqzbuan.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gdzsyrgaz.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/glsutkefk.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gpallbjkb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gccetchcc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gqnugpppd.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gphamxtnm.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gcqprniwp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gxrukkgvz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gfxcyxykd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/guhijjttw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gcofczser.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gkzhxvkgv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/ghbujlqba.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/giitihjiv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gtjxxhkdp.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gmodmigrl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/gburaqwlc.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gzkbogvbb.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gnygtvcht.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gyumwahtu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/giclrnbls.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gxmgkkcez.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gtafaqgbj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gvbupzcny.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giujobvgt.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gqwnpqput.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwvjnimlm.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gwmbfosyd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gnafayfyz.sHtML


<!-- 参考信息 -->