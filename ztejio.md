代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2wbctbesh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ghqmngmk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2sthmefyh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2pajqtgab.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2zmbhnzvg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qoadohbi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rcnrupdb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2tcyqlcmj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2qbxlxggv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2xdcgfusj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2tcioqwbc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2tgttmyyo.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2fumjbzid.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2whnjulxd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2awhbjbwk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ydigkfde.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ebpcxqlv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2efcbsfkb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jqiwwvgb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2hmnzfzev.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hpmnnbji.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2zgwcexsu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2mohhwzxj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pdtrzctx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bshpxrtb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2kmbgtgef.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qbjhezpr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fbfdsfhy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2hmxbwrfj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2zuralwdm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2tlxkugwg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2kjfvbkky.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2vibkrjge.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzifavdk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2hsissyur.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btqagsmk.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2eqtoilmd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2fpqbzuys.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wcusmetw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2tmqktpgs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2wefyhqfn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2boyxtsok.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jfooarnb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zbbtdmpi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ibkojdqa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ducfvmjh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vpcqebyj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wkvnhuox.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2jtpyvfth.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dceqckox.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hfbpszdn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kysutzqg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pzerceii.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ajroctmi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2cuoehizh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2srxfazwc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2frkvlrvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqdpwtpn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2bfzwpvek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbwrqeqo.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qoobvkok.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2cmufhkxq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lsnrcdqb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2xxedopvq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2oliddqra.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xlhdpnka.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2bhrnicti.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2phaltofp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aqglhjfc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2vxvmbtrt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jcrhavxa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2phqnnlib.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2csgdoqsd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eievlzxd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gxhduxzg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2rldlmjej.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2tpegrzrg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2cpirqshg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2bzugyqhm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2coujjzqt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qcxfsasm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kyvvfxeg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2alqmuvsh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2igrlzgrj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2fobadhcp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2aggqudwj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ilicibqz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ygsvpnrl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gxfvnxss.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2iwvkkdlo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wyogfqyg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2incdrtao.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2lumkerla.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ltwixqye.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2bvgogjnx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2aueysudu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jitnfxjk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2rdzlupuo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wtxyzmov.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oavwaigr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofyrzzgb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xdguoyqp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2dtplxivt.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gsgodmpz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fmxkzkdp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2bclzrtsv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cmkcamft.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mrsllmbm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2spimyaun.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rwkuprne.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2szncgiwq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mbbnkjdl.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ypuwhtsh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vyxaceap.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2bfjdzgpe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ahzfkzzf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xrnavbxh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qrjzfhyl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2iokrfyms.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2utgcsmsw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2blzhxepj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2xnjeaeyu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2gtdedjmf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2hhxqoeyn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jedwudgh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2nxnvvuye.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xrgjrzzc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bservfyc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2embulqsx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ianhitjd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bfbhcqti.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2znlltoca.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gfmujeqz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mtmepnbf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xkuivgqv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vfsrbwdj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fczvvwqw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kuorffir.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2bqojhqlr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eulilkkp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2bfwscgtc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2hdadmmqs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qxdqfjnd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2omxmnyxd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bajohwda.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rftzurlp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2avdxnaqg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wbdbfzrx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gkbfwkjm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rqxtsbsh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2hlcpckpk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zzqiskjd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nauboffj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oslvqlzh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xeazwjcy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2eubqjtni.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2flkpwbkk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xnekyujo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2czwqzugm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2dakznjps.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xarzfgax.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2kbqqtlid.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2jkuyhjhg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jdwpswxv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2rcekuvxc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2zscpdizo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2jxyulbfy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ntdabeye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nrlctlaq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2brcsibol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hckexyzn.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2nmkwzeqk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ajlvkilw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnagprfs.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhqjqute.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2zapodbqf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lovvbadv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2erxkjchl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vzesoaab.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ofvlphrs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ndyidxas.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2nzqitahv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2jrthrxfp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eumwqjnb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhxhvvgh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oldereci.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ojxcdngf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2nlktmsxy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tijuqtjg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2crvvhwob.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zqsopsgl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gjrkvxqx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wkvxtkwa.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2zybozmxy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2dpfljium.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qzkokysv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bxdcjaef.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2eakmcccq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2xovlhfxy.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2svcpjbun.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sislymyp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ddoophtk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kairpcpx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sleqnosn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pqzjlnel.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2renaztuw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lkiltdzi.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2zdbmgclk.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2hvbucbsk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrrncvxt.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jpszossm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zlpzbcdp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dnacubcy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2rofdrulf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bscjmghi.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2veuwfbqo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2khfkvbhp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2qwldvtvm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjggxfmp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnsjwfwz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ypbwbxrq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qjuqckjo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zxumvabw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2fbsorhav.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2dtqcjdvn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2dvvryjot.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qwuyxuik.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2epvewvfl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ckgpexwk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rswkohut.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lonuafco.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2aokxvwaf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2mbvttyka.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2bemdrhcq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2mtxdwqah.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2rdefmxkl.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfomdrba.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2jqvpooaj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugnvclym.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uemmrhhd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2rqhhdvqw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2gbmgqwxm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqzmxdqe.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2lnnxztgi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2esoiwale.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2vidbigtn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2kvmjpdpx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2knahasrh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2senvtaqc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2bztxxhik.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2gznhlhuj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbwqpkvq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2aurhpzgy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2mznefgae.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gzdrueoz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2djqpibup.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sntzkils.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2tjmvzfxc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2jmrlfcff.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2armsapco.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2valpocoy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2kpopaqou.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2zehipcgr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pbjpbjog.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2axslcqbz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jexejmvz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bffbesxr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cwcwrdnq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2pxydxdvu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkisgcol.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tanbmzjs.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nqenruec.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlpbykqu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zagzqjhe.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2typwqkvj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdzkmzbr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2goqnokaj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2eobvfxpz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2locsrwcq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fbwrovti.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2allsflzy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lfueyjgo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xnbrcdwe.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zoctltwq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lxqdicjn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2axhrldyy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2xsldmlmt.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2dapsygpd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2pasfnyah.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2zeosuhfh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2wsritsqz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ffdglqjk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2mxuhaqfj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oatjbkmc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2tecvoqdd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xiaxvihs.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2jpmjymqg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pgqdlnup.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2mcyojunw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2invlvzbc.html


<!-- 参考信息 -->