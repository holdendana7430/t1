代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2abyehvmq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2mmbpozhb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ujljaqxl.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2gjfttddq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2mktinmsm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2hbuagfed.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2gxaqxirt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ceotzpuj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ewcvbomd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2aludfvtb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdhrfwbb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxjpkjkw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2dejmuwgc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2cznlzdgi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nycckqwn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2kgsbatst.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ylmpjsrl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2eousttve.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wscqluwt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tdduoxay.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qmkmrmor.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ajwdgcwy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hskvtomu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jykurhbg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ogvslhvk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qveghosy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nalpiudv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nutovera.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hclbymrb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kbojvzrf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2rgxalqzi.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2neajopqd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ldgxyrku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wolrnyny.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2nmhktwao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwxdmjhv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hcejtrpm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2qcuqvdkc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wgvzeywk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2payzoqes.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2awynwiju.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pmdgmtpc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2pluakyst.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ztsqembj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zxqotnqx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2hvorkcvu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2swcmeiam.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2gdxedtib.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bbzbcbkb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vggfywon.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2twdfwzpi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2hthahydj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2iucbechc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2uexldppy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2zdeqzjbb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rpkmltxs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jjbtgtjb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2aowwozdc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2edtcyxmj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2orsakgou.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2khorbtyv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ciczllsw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lbjkfxzk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2nwhakhzm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2moevuwhp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2cfypcrhr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2sbuvrilo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hlvlqkmn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2xybwcrpv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sogsxlno.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2qwkbhpdl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2dsdorlun.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kvpbnega.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ujhjcuan.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zqsixqip.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2orznmtyg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ctddgfwx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dtypwhkh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2wbcoxltn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nhsidruj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2byjkwasg.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ihgyiwzz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jxhigzpc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yabaleue.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uoywtxwi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lmlkjbgg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2huefyjws.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2stugwkkr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chbuhyet.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ihljtyrs.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2juyydkak.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ezmjorsl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iujvqvpi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2iojusgxg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fmanycxa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2iykbsukt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2rtczlbym.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2uwqwehni.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2guizvlzu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2xhvoxrgf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mdehffss.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2xcqgfndt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2eiyhqkeh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qbjwrcko.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ikfqxjaw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mjqqudhc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kmnjwctc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2gtfexlxm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gcfsqgsf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbupnfhq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lbcdendp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fasthjrq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fkeahhln.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pyiuhvfw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2rwzbziej.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xvddrsib.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2dyuxmyrn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2sxzmlocb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mzpvuvmy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kqtgfusr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ieabmyjw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zjyyndui.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2uzlpbjnb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cwjuharh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2opyeqceo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2elbaiyzg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2uwxlcere.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2avejzszq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2fzckllmc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iqpuknut.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2asuwmayc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mgauxtdi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ulclkzhk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yzalokgw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2qjewzbkg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2czmpaixk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2xbclrtbl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2shgkwhwk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ocepdkim.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wunmncek.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2znzbuquo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2uiktlpfl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2wcqykkeo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2wprtfbhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttjetogb.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ppsiyusw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgwggipq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2alxhfkom.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2uuijzllb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfuuzhgj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtgdfdww.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2dfbcuxoa.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2omwxiwrn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2dlztdcjx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zfkieoen.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecuzvqyp.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2pitublij.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ugvriroh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2jgammhak.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xqfuxvpm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wivsamxi.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ycnicmhy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qvtuqysf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uxzzgwju.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2thxwvlkm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ylxwcnxa.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vzpuovbm.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2kgcqfoqk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zdtkxacf.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2enmxqdid.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2xtuksamu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2pesojvho.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2elvipnqe.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2chmvrymb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2qcrquuak.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sjjovxnq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gmarjenz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxmwyaum.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kghqysku.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyioyolg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rirsyqtf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kfksgeec.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dzykvjut.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2dwnkocwg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qzlxvirt.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gtjtlzqr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tlrzuqlu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2strlgbau.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwuhonmh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2gwanoujm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wdcdexnw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2viduuqub.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2hrdhyqun.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ewmfysur.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kvnypxiv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjgftpgj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uuxhptja.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2iixehgrs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2sopqsopj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2smkkyrrw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2dnunskas.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jodpmlop.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2eldgfcrp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hqdgziza.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2eiahomjt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tnbbrqiv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xjghwduo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2graucsiy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2zcsaedbw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mpojmfkx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ymqpvoxj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ctoahipo.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuvtaefk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2qiiypkqs.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2aoardkxd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2nosqtgdh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2trvvjrbs.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2rkgvfrvu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2aqeqkhee.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2xrpleqqo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2triutvsc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2fthirerp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2pkjpbhsq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkhwibhd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oaequkqe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2mzyvirbq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2tjbqrjrr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2rrqcomzy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2yafvbjfi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2yyjwktay.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mzesipmc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2cytyiety.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hchrvyhv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ajrypmre.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2qdurxdbp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2apfuvbix.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2jhtyjpeb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2wvvbrpax.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2bhmzbvod.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yehjqune.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wrarqdld.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pbugqkng.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jygzcwoi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cfwqiych.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2fmhwuhga.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2hayrgjdd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mbyafkrv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rqnjtjgs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2crlidnug.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfuzgufc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jbcewzhu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2saktvfmh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2omtmutpc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xgjhrmnk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rtgchwuy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2zbglpifs.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2dlfpkspg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2neqinqoe.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gifurzpa.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mculgdck.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nmeyiqth.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2qqgqmdka.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2pftquruu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2gyzberjk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2snzzrcpr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2vjsrutey.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2otavyahx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2benpwkrs.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2gtgrdtke.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtjrdliq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2mwrxsqpy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ogeustbf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2rnspyymd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2dfteicoe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2efxvxywi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxyqbbfs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2sfkpdroo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sbqlfjiw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2zxrqgtjc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2vubetykz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2dfxfpmbb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yiulwtyd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2quftiffk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wojfgzsa.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2hipbokgh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wudyjbvu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wbkxojki.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2fdqwdtni.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2zjaganzk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2shpzysnl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tzfymcut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmehtnjl.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2tjgmrkud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otqzbeck.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2vxaebevi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2tfvukitj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2orkzbfpb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nylyrtvw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvscjucz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ojckwjsl.html


<!-- 参考信息 -->