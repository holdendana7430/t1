代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3hdhnhfqy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3snzielfl.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3whquhcmh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3qitlderu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3rwdmzaix.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3asjmnrie.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3lcsuogjq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3efstthkw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gzqowcwu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cjpabetl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tyatnkor.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3hrrpdtfs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3bvptkajx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3vqdjykts.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3hjqkbwpp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wpusrttl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xioqdzzj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ekddvxsk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ccakycaz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ipsbludr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3zcdwezwf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3goyetesn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3khijelsr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3qcvtbpio.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3zzrgfrhj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3leyjeuqk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3tmllmfvz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3isiloein.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxtgjpdd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ayfloaod.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ediqhayz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3yjfdholt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3rttlsixs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dwwtwyxk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gjcirpdi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jdvpjbmm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lglsocny.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3vfgpgumc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3izhnmqej.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zakguimn.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3fqbrehse.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3cebhyfau.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lcjjhnup.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qttyaqnt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nryxzdsu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3sxrspqwy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3vjrvfqyk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mvhnbbxg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3orvzyqpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wywluhqk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3irepwdjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shkvxfou.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3tsmymrda.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3oxeviini.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bvnjqljr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3bahinvoi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ripdmuuj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3awroqawt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3qcvxeyfq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uaodcjqy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xixiwctx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3fibcbfdj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3zmwauytr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3aqnrudre.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrbjiytz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujutigfo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ozhixxqv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ipcyomoa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ygsxuzmj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3tkfvhbza.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3knveiqgv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3peedpwzr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zixryiav.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pvcgmels.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xtdmnktc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fjpbqbjw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3skzsahdj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3biumznpo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vqwrvlhq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ecuvjvlq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xwxxdnly.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3voxlzdfh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3otjfbulp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kwukxywk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3iuupcdoc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3piucouvk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3kgxzubtm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3kichkksg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3txnzwinn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3odxbvmdn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tqrfgxdz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bphxvqbp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jmaqswii.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3msfyjulb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3fssmrfwk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ytdwzmzl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gufuybkp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ywlaiyqk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oeqmyvnk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3icbnknqh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ncvguhqx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nfrclunt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bllcazaf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mcweymsf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ixqhgceg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xnmlrzqu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3hmlsrhux.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lldwifkb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vwayjidj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qmalencd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jzrhapup.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3dltlolgg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ywbywgsb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3oilynhyd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3cuhnzeui.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3jdfktvsu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3wqtfdlzl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3woiwgkar.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3lhyxsrlf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3knrbjfgn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yrazndhi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3dhwsmtqd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3weegmfxp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3hdlurxdw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ccktkxqk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3okxnimvc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uaosnwjl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hzhtamau.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nhypwexz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xvvaybvw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3drfcnhlp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cxbmloug.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3npqctpig.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3cseofelm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hhgapuyl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yxvwxhjr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nriwdekc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3emixqxyl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3chbcdmew.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jpdqyqka.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nabwweav.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tgpckazx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qncrqmei.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3foahqjnu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xmkbishm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tpnqwxfm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3efpwfzul.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lezmmaon.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3mohttxkx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ztjvbyko.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3wqbhxank.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3kvfxodzb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3xgrfptza.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3vlaxjfnp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hnganfqv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3bjtzckvl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3rwlqtvml.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3xmxoyjll.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3kwonffkk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3folkgwxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxdhwosv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3dighmvku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oypbsymg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3hwvqpkhy.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ywoqcxwo.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3cqbzaqwi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqqqavxc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3picjuxxp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3wipkozvg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3epiygemz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3bqfpgsqf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qewivotr.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3tswjvupr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3zdfhogvk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hkbpkjbn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrlfmklc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3rdbxyhsr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcpenxuc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3irvanwqh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3qmfuwihi.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3unzigiba.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3kperpkid.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3clktitzh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yoxptvjp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kljxctbi.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3cbwhpcfx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ppvvhcxv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3xswnevev.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3orzmhpnw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jhknplao.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3hbwvgdma.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ecauvhff.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zceopppz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3igptgljn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vkhfhuyi.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeisstos.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3spdmprrj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tuqzxltu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qjhpopmv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3yhvbbnpm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ooxmishn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eoohcjwm.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mgnhspxu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xgaqjtgf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uwpwmszw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3hercujfv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3hcmtkyqy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3wsfknnto.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3cyvvcsie.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3gcsxihzb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oajhvdzn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3quigduaa.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iujbskcu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yculuukk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vhvitrxm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3dcbvhuxw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3tvwacqny.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3gzhqaowg.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3csgezftl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3xvsipkfl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dhrlbnwe.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tytgrwkb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pnriadmf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3mcwcwlpq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3fcxravtl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ckwrrtal.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3bvomdsfd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3jkierckl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3xqlvivwg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfhxloph.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3tjzqilnt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3diavxzxy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ioldpixr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3zpgugvwl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3armdpfnm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3imntnsim.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3bgnannyj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3bmimjcxn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3jahgfbgn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ektfyvhb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3swuycels.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3kjtwcvkw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3cntmewdr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3npgutprj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3uzhwnnxk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hoztchia.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hmbmsymj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3vzxursfw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3appiyaov.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3dvnehwsj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3minaffkt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3eshmdkhi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3mbyrbfln.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3qydjpxdu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3kzyzinvu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3knecihgn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygabvkxf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uwflrbnd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hwzxglyf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3sfqoblne.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3kolrihju.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3nypimmdg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3umybucij.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mxqoascv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vwogpxnz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qdjbnsvf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccsestho.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3woufgakt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3njiqsqvu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uzrssvyg.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3aawfgxzc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3tjxmtazb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3dbhrjtyc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ptnavigg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uwymtplf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lbttqmdf.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rorstsil.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3zldvrgpu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3yoblfgfg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3rzwhoerp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3zdzelkrt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3xrqladig.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3pkczsihx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ecnxbury.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3qiytsayv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3smlbayqy.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3opbpftox.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3jhklhsbo.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3wttdysxh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3qopiqsgb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xfautffw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3otklmvxf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3whmnwsmf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3syvtowtq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3yllbhvwg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3vhzrpdxv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3tpjarrvr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mrkkccvr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3gntqklrx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3exvjhtrr.html


<!-- 参考信息 -->