代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2dokilmcf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kjomuuoq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2nngaoniq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bogvowpv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fzkhnauh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pzxmggbn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uzreapne.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yofmxhqw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2magngoew.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2yubvxzlh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2fqkucjna.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ezgkcyyd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2jgnhofvj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kddwujne.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctyjyuxf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2deqkebsw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpfswftt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2obgdbnrf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2atksoqyh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2lplspqby.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2wluouyov.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pgsliysy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gqdadods.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ihaihvvo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pwfwfhus.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2wgmzmena.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rspahadc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vygopmae.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2dlgpzucc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gkrdplou.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rtsrsodc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ouqkxuau.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sxtyqgzd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mhdhsjro.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2mwdxkypi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dyozyuat.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wpvjtvkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmzvfsql.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2deiiehpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sxfhbruv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mibkgbkg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2vecnhosy.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mvowtmgo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2fpghfftx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ndoxefjr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rwejluoo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2egboufdu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owetqofz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jzkgnphc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2lbnimmpc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2xfqwhqat.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghhgviey.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtfnxflw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrqcufco.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2oomlnqkg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2yimgwlrt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2fzowmunz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxhoyofz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2xxkevuxb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lbtggxac.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nljehzmi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lwhhmknb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2smcniuem.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fyqnfgdc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2kfmnjgla.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gvmlpauc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vwayqoky.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zvrqtixh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ldfntzkd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2cmooqcmy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2imcsidkh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yyjfuthx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wntivuqj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2adorardd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2qmvfobjd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2eaafvxnw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2bsqucvte.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2qkrloonq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dcujjuvo.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2guzymfxy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hsjcpokz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ordcbqom.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2zxjrxbod.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wbzjyngw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vxbgundl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2pgtvkuvn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dviavhes.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xizrcssv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kqqadwwm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ogjgpbrn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xeepehfc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ccnjafat.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2amhuezuz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gddjhgsd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ooohffjy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2tittjdgk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gwjpjlmt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ficxjqrd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zeaqytgz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qfyqglih.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2klpytqrf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2muflsmzj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2qnnhwstq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2byhrlswd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qbbjcrlt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqwdbczz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2exmnozyf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xpitbize.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ydibyqjb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2cbdduxnn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2itxkpvov.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2xthaqkkh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2nmlqwesu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2otmoozoe.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2catajmif.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xusyhdyu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fclnbksl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eezdbxzu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2yeatuhvk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lhijusiu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2jzeygzlz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2eunpgdli.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjciddsq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dcpjdama.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gatdpzjb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qhupefqx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2tacpzyfg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2paendqff.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2scmdsspe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rlblhzlf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2tiblghkr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2shokmtya.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yytxbwow.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqqqoxkp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vkfprvlf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ylfkbqwb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2rhkohhxq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ltqimpkk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2opnpvito.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2cvdevkrd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2krrqgopg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2tkoulbdh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2lkmypbrh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2incnrdpx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2epndsbcu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xgheilxt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2tbhimzuf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2gbvxbphn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wavsfrdh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2dtvxlewf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phluhadc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2gjskevwb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2cdtfjwdm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2jantbxns.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdfntvqs.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2fljreyps.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2imtjospv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ckzfwnwg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ahicwkug.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yapchzqq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jewvsvlc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2uisukslm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojuxwesb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2iyuwmksm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhyngtkh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fashmzmi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2mynlrwpj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hxwaijxr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gqlsclox.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ygaqmedz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nmrxoypq.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zblogjhn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jqfhbuap.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jqowxetg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ecmwiqiw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2crmaxrer.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vcddtslq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mtpjwrzm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2rnrjbgpg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ndndtyqh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2erehdycc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bfzigotu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tbfejzoh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvylzyhb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ibojoxgl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2olnmqqoc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bfkridgz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2woumzzfh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cjhgtgya.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cogazajo.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2honharfz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2frfhsnvu.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dwbxtsbj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2izofkuar.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2opskcbdd.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yccrrehh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2mnoypjjn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2jyfuosjk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xanuqcnc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkrthyvs.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ystirqcw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nipxopbn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2pjjthesp.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2gvftkhat.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2pffpzowb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2asxstlej.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2wlgnnomw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2quqbkoho.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ifimqdln.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tovmslot.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jqmiprfz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2tqfpimpq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2fqtliaok.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zrlkaamn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2rntzykuv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ubglbphr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2oxicullo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2toqcbwaz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpxjspph.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2zjtctkrz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2fvorhgvu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2yutwhyts.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvdgyebz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2jscnxhui.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2bdruuuqz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2vwzfhfxh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2enqbcigf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ekfraqqs.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2skpzxsqw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xtrlbqku.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2zojztmpt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhmgztdy.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2potapgwz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2vlieodpb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2obgguoqj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2owcvcjng.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qwbrgjix.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ooinzutj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2nxdxryuj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uhagnrag.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2oaolupzc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2noqpacxe.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2vrziipka.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvaqudge.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xzhmhnea.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qyhwdzcn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lalarolb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bkbypfeu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2cybwdcwf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzhqzdiy.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2fclinoog.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jfhyutsp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jjnyzsim.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ewqmchez.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2induvpcj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2btnmlxzn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oftncwsb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cffiwlhm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dvscyvcq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2cvmkmggr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2kgmsevah.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hrrjnywl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aqcprrrj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eabseefc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fymbtvvy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2pgkvfbzc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2azmrssxm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2chbttdel.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ldmeyhaf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2guagdubv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2aovhffxa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ywzqazgl.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2tzrlqkii.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxrffugz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2sohrtzni.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2sybpektc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2xnfqmahg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ktbjagqo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2tquufpxn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2zjzebdsi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2tleiyaii.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zebvbllo.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2awpjmddq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2bxizrpit.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2cxkxchry.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sbsqtsci.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2prxomhya.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2vabhzwit.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2mzqjygfw.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gumnwocq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fgpnkjux.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2crwrsirc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2rltwoeya.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2irspokre.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2bqmscupy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apaqpdlh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2hgmtmqki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgizjfgs.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2xncfxjnx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ldxdzuia.html


<!-- 参考信息 -->