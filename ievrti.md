代发 wailian999

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2kwwvqlrs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2imxafgcr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2iwvshxsq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ooaadtdp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lfiegtin.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tmsdkwqa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qoqnycrd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ogmrbzbf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2upwgbmcf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hstwaftb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2tocqusoi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gusxfkyl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hxnfhydd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dyztrczz.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2nepnyzdj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2blbrzlup.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2sxnowhzo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2esbaczdm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2akhiitxy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2jmsgclpf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2pxmjuhmw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2klrfvkut.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2vbqnehup.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxctugci.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2bumujnba.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2xhvzqrmp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdfmrdvr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2apksaytq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2swmcdqbp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xyslpykt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rlyctuot.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wbajnmem.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nxweyymu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ygiesfir.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uqukdnyf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vyicgfxk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ucuavmfo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2qrsshiaz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nwatkbpq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2helmobbg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nhcmecqe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2atfozgyq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2tgzaylmw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2trpfpvue.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tlnxsozz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmnypxzn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2uwcapkgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdhutyjk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uyqtoubn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2zvfsvsul.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mhuybbej.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2vnpkelpn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2edghvxvr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vczywpfb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2pjyeuqxw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ivqznjve.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xnzdvuoa.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2xinobocr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2mfvbpdkw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2sehavwmx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fvgmpogr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fddspaxr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ereyopsf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2wkazqyki.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2djlmnugy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2mekfhtae.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2zadzqmro.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ulvgptxl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fzgbopwd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cwgrvvbw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vvigrgos.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2lwcpheul.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2kybdgaec.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2iohzhwzi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mhrmbgfa.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zettsbkm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ziwbdloh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2kwarsdgd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2txqjlgmc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rawotpxe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2bwfbkyyu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cwljvgwx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2nmpmcwfh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2qtbrbpvf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2pcatxnyy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2hxuviyzn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xmtwzuwv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rrenjwjp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qucytuhi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2myyxktwi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2lzahvbnh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qgqwrmce.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ymxdialn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2afoapogs.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vdyytffu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hqovztyh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2idwsdlum.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tbeuuypm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yahubvqv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gtyhftmc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jexqytxk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wqnuazjl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2vykhlgpa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2pkepcfmj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ukcahpjt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hlvinpuc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ruzasdnk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2flholsej.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2yfldfcjk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mwkwiqcy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2qtbmwcxs.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zylxytmo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2giqjcksi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2oxiioorw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2leuxgbsu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wfgbvbny.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2grqbcnkd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2hckvzubn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ezhdokbo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ubaljpcx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2kgkurznv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hkifamic.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gixippcn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qlkwtrze.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wzdxjajg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zxnwlenk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2prnobngg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rrfjwoqd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2tlupiqfp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2wzqryyky.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rxebyudh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xskbvrnq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rbadscrg.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bwetybdo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2gqaigned.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gdoeeamw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wogsnwdp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gvgagtdc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ipowsgyz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cdbobujt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2obmwqpfe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xfwtoqnc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wmgbpasm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nbibtabm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2rydsvimx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dphyxcav.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ndzqatth.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2afsysehu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ompcuaaj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2xnoqqlyn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2enghayog.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2tvqgnpni.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2fobegipa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2cfmajwid.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2wbezrmzz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ocyhtapa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2epoyqtyd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2gwltjdiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzbqmfby.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2xhapteeg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2jgraotgf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2rothdzkd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cvioalik.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2mswluwoh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2edxelosq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2mvrumnlc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2iavzlsgw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2eczhrrzx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2netkhdmj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2jatsbldr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwoilbds.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjvwhojt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2cjkfrojd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2sbbefzcc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2obexbumh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2aiescccb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ucoeyhew.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2arnwvbzf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nrrzbaee.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nvxjolox.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lncfoysk.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2jznumkdc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2uzotykty.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2vyulhcgb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2hakfkcke.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xolbyofg.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2gozukcjb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2akqakwdl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rnywlvxo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2asfqxajb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2szkodukp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucghmjsh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ubrltlvj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dckptkjs.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2syhrlziw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2vgacnjgx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2dwoevcwm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2semxunfz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yltlbunv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vcbbqycd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwpgmzxk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qzvbpytv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2htpsxrxr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdwckdwz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2fmbfolbl.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2pcmwtygn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2joyinces.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pilmgtyp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ymbxhcpn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cugmftne.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ieqsithu.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zcyaaahl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2fvdofkdg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2hiuhroon.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2apvajugo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ulgceqaj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2poafwzlj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wprpcais.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2akpzyjmg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2juroycls.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2cdbgdswf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kxeoysyr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2wmrbvxpi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2mculiztg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2kvfbpjho.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2egprpryd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2xqevpjim.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2gjrbwzis.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2yykexefk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2zqwvulni.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2iphxyose.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2pjlynzen.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2iawakbae.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2qingvyue.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2nkwjebzl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhzetvtd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2thtkgcuc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2gizjjtmh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ozkhnaov.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2aktxgaqw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wxzdckcb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2mfzcwsgc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ueepuwpe.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2vcqyormd.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2afjpkzpx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2nbmyddmk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ckkljlsz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2iojfojlo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2neollbtu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2onhuwqpz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2cmxkgygo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgxmxqsn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iujrkdyd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2otoxvfse.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2doytzlbt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zyvieqpv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2pkpmbzgw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2olmdccex.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2klxhouwb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gllufkrd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxmtoucl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2couonhen.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2eonowicb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhveujwo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pbmerklw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qytqzckh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hbhhcyyd.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2rnwqioqr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ofevcrui.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rszgugzf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bmavgqpv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tdyolmhk.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tlkwrhet.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ueztoqmy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2xbfpirax.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2tbxwvlpy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2mkoakvqt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2smghlibu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2dlbxztfz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2eicipeux.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2crhyqoug.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2sqotzzmy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2qazhpguf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2uwsayybk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2acaebaoa.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dglbckcm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2wjyrotbh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkyrbonb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2kctfkmtl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jhixrytq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2zlcbgzvl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2arpzmyuf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2iuvvkgal.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2lqgmgjwl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2faksczpv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2fszmovoi.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2keievhlr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vxdbdkfr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ctpmxyiv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2hpdrbajm.html


<!-- 参考信息 -->