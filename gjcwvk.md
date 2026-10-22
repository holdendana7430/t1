代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2bsiephik.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xffterdz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wqmntvtj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ixqxblnr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2luzbraok.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2btccwxzs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2yhmcbiek.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ozhlcymi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tnrkwvix.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ydkcyecq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ejulkquf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2zacitxqg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wbrvlehg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2xghdmobw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2rqluxifz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nlbpqdaz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kxqkxrtz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2slzhjspz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ewrcnmzb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ananbsap.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2elhsyqls.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2vuwdedyd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2bufkydxn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ibjxnwtu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2wftedywp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2afixegtc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2jiswhvfk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwunbhxy.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2bykokmzg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ganfgdik.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wyopthij.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2pekcroel.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2zbuzjpeo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qtfxoaey.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ujnlrcoc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2skyigdny.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yxshvrzd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2vhxbiybe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2askohycp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tebutsql.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2wqrtfgqw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jivmuqhi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qdsjnfxn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bubhsomi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2duipjqwd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2awkzrqlx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2effajnwf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2waubulci.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2amhpmowc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzeyuilj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2yenouggr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cepqqkol.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2bpsvntql.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2btdwfgjq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tgmypryg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2jynjcuhd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2goetpdgf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jfvngeoy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2skguhftc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iadbbdmm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dlyvfbfu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2unbhsevy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ofkwqhiy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2lmttfjrh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ssnxuzxi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntmcnglo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pscdbupj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xnyfxena.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2lobtwupe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ahwkayjc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2pgxbfikl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2smwkmsah.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yyrukqmh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iusxmdyw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2asscqgqp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2fsocymbe.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2szsjuccb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xllrhmma.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uonaqzvw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2uguugvac.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pdssreif.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2oziuzqaf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lhkeyquf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qtrkvdel.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jltsyaxu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2oklfhbjo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2fospvsou.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2lopoxfct.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dtuodxow.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tynnbbxk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ummfmdse.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ommcmpvw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ljdgiyvs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ctozevrk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2agzhbegw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gpgogvhg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zmybzgza.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ftaaeofw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2srtqviqa.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dxejbiaw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mtyhacwz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2alqvdosl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sgktullu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kdkywcow.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qmgipbbw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vhjgxlru.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jwdpuehu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bsbbcklb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2eltuvpcz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2suuugfwh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rdhggwqs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2oqoqaunx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2voskyihm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ngugonek.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2kbizwkgj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2tlgwqbuh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2phqdidju.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2jxehphnu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uxzndqac.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fnykirjv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hyuddkjn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xfzpukuj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qpirdjem.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2vuwynnfp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2lbieatlx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zobtoplz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yffxnasu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2anjdgzhf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ntgacbwg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mcentkal.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2qgybinbz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xmlalmiz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2hbzivcix.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2csnbyvep.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xifqgmnc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bbxjfetq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pioqltue.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zzfcvrdj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2nzkjwocv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zqecmtqh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqkukvru.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jqgnwdhk.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2vycjihve.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mxxttjcv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2mufefpdh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2omlzrykh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cvqwnspu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mmzxhbpx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2asdbptlt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nfwujgup.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2tfuiyakg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2wsycokid.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2croexkem.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2kkbkafuy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2uetnikfw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ndpoargl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ajkgovrc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2fqbuyuya.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2sathhipm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2xhlvvzsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eaytohyp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2pmhclsfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zlzgehvb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2zjaagbwm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2xfaqfncd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2jjmncvun.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2klgqfuxc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ylzqqddv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2irctogdf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2dyzldcay.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xmtmnwak.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qnhfahiz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2rnrzvifo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2jqubfxdu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2coffatyl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tfhenwdf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvxvnzxf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wsypymte.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2twbktuho.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2oequsaua.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2romzskra.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ogqrrjtz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2avvskfcg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hcfqucch.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2kzqazokl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2rbugymak.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2egfbgexc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2kjlukevc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wkoeytxc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2yggokpfc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2pxholsut.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mxmpbksr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qalrtaor.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxdnfkpe.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ywlrongm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2niaecbji.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vaznupmp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2synuuxal.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kbyhexdk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2nrptjleh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2iismpbww.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ysjcphwr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2suwuvsnv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pdgfjqjd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nbsqsnzn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2rcyyvwye.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2tgfvfzmd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2giwlbukr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2rryrcdmo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2esjqkhzb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2adhuqfid.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ppewpmpc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lemihwfu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgybeqoo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2fuqedhpz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2asonmhyx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2fiyulkfc.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2vjwjyveo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2dfruedav.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2abwetuop.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rklbdkdl.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dggqujpu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lpigrbfq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ewojkxqw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2lxztfnlp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2eaifwgth.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2szznwijx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2moewizle.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2fmxzupze.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nhuziifz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwlelnhr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbsptuly.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2wehsrrxh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2wbmzarwx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2uylolclr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2nvldjple.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2kxqtftkk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyunkoyk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2vtylajua.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxitmcap.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzgpxkwb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2axadpazo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2wtvymvhv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2eueozmsl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2igqixvfq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ctilacdy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hdmhovhj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ythjnwyq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nddkszic.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2odxtlyxh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2nbbepucp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vsdtholk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2elrkckkq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2heefaejd.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2rqpqriig.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aatyyfwu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayxoukiu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhicduhm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2umpzxaxe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qckqjizi.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2jkyuvpsi.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpbzxsfr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2boxhpkpu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sybbwrhm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hitoyefz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2univoess.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bwklydxi.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ieqpahig.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ahgxbpom.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ynqgmyoq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2glgsttqa.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2eezgoicn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2wqpumcet.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wrqnfrqr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2webndfzl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qjoapypy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ljvshxpw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ymvtglzk.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2axwmiguv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2zopmetyi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2eayzgtnl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2gnmhvjhh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2rhimqlal.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2jossblkf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2qjwabsmi.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxqvehgo.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2lkretxve.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ssavtfah.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2davxsmad.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2yrprhxap.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2idffsqbc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2weryrcdl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2rltsvuzy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zjihrbsm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2mmiwduse.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2tqwzyqmw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2tjyevtee.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jgrkzrbe.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ivxtonzu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2vxmtihyc.html


<!-- 参考信息 -->