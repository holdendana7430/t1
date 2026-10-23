代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ercshhka.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ibfzsmxg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hyqlorcq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3pyxrkhve.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3gqqcotwx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3beuopwbs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3eqknvhwd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ojfkgtff.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3zkonqdmc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mjjtzrah.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3apotobbf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3fvuokonf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3eybfimgv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3erhufvzw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xsuxvubv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3irrwnjlb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yhhaachy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tvluskru.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jmuxqdzo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3adyyglpy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3byfuwbbh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3niymgpox.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3cnxdqnkg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tilxofck.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3immxiuky.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zrhxlatp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nzzsmhlv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3junbbvah.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3tsntrxli.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ytsxqhzf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3xqwhooxs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kbkbtjjm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ddbcsdba.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ltgarhbu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3pognhpme.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3szxoenzf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3tlmkyhpa.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3jdfhrynj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3zfoyurbw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3icskenwa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3adukrosf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3qjevfnov.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ipagahvv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhwfypkl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3kvbvkhxl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3thpbltca.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3byiqgtut.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3pwxixvzw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3xdjsncqp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xbkrgcuc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wrwjtsos.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rtazotfd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tfofxaqk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3snmiaucv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uncfssho.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ekfdhbaw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3nkftgstu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3rfkztuft.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mrcgjyjq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ltejsvtn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pygjytuo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3iccfnape.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ccnlhjfg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tbkeztwy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3rvcvwtcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cmslxztl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ftsnskgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pdxodxtx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3rcnndpfi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3jjkmqljv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ictapvbo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3apyqruyh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3oiemogvk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hussqdij.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3jbniitzx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qanubolr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xydaajie.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3iwmyxizb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3qvnewnci.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3snnrrvrz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ourbehrr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsenzcqw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3quahmciw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3relbhxjw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3zsifogld.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3iomhnrge.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3hwlbrgjs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3soqctuhw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hfiuqzat.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lpnuscso.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3girhsowu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wrsojfgh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3bmwzazpr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3rayogvmf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jakncned.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ubzoflum.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cwquaijp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3bpfpqpxq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lzpiaqrp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kwmdsjpo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3fckdfpnb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3shzwuvrp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ynerpaut.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3qrhgttjd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3phqupmpj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3hknbsdno.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3udqayjdl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxyvhwkz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wnppalnn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lsgjghet.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3luaidkom.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bcxrismt.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3etsitjvm.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3bnkitkyh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tzinhxoq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lgtltfxl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3krzuebvj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iirsjaxv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3raxvecsn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nfggjboz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kqdiselb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rcflgclz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3cxosnnkg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3uqkxnhyy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3hbcwimqg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tltoagyv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wreoyirk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3otizfxaz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jdcgsiof.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3gbclufjk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vovzcoip.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3cwhoshct.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3peetovni.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3gielphmw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ouoyrlld.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nfgoaqqo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bnjsrvas.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rtoysumo.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xchegucv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3zowdrdhr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3merjbgwu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kfdurbrh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iyclwuks.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dwlxazwy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lvjgsylu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yojznqqf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3uekxklth.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3czsausoa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jveuicky.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3wxqszsln.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pvwreizs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bxiioikn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dvrozgxq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bdyzozrp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ttqtlmgj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eowsderu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vbsbeqqb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rfuhixku.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3fehspycn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3srjsfsha.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3xwpespcv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3alnzedyq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uvjvvwzv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rytjpyjr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3axdedepv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3itvnacvn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3hcpvgygi.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3wvukbtnk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3lgygjzez.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3sprybmdr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3jekwcchd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3navmygnc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3rsengdyg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ogoajdct.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3tpvxehrr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3chkoeavy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3urwudnux.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3fjjyrqcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjcbnbpe.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3eekcwstt.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3lnfebrry.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hadjvjri.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpszgtqt.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ctgripze.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnkzqlka.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3tevwwsfq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ybgfiaiy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3olgrguui.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ojrztkqc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3lhfwuuqv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ssfqnurd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngekcioy.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eoosqfhu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3opywwbvx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3blwgfxom.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3siupcfsy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3evvkfvbd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3tjhjzuuc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cunqdczf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cvtjowbt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yctdbaju.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3idnmzvaw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ckjnkkor.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3pxaveszy.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pzufjhxx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3dovrbdag.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3juzilfpk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3htkywkax.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3guchfaek.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkzgonaq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3apivkuhm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfpdrrsw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tzdufzvl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ppaxkwoy.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3fgltotry.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3chbyvlhe.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3onfpmvye.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lahxpspg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgysfril.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lvuwjprs.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ogddgmrd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3dwbmejcm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ypkoeuqu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3plhgxlml.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3phijwkye.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3nprofask.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3titgkboh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzexrdfc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yegtgfvs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xowigggd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3thvzfrwy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3uqnvpamp.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3cwnaxzrb.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3hpjgknqk.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3opqvlhdf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nodsmnft.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3omlgveyo.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3haddoxvm.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rtwhqtia.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3yicdetdf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3cimnbnni.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xownoigq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3mpyaulsf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3plsxuofg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3osatdmym.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3adgugwxh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3gdeolysv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3pnwokidi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3foyzhdic.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3qmcsiaoi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3detadmyt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3mgtjywiy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3rwygqykc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxkyfmvg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3wyeqqkns.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3zrbqjbfe.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkknsahe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3llcepxar.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3tpnggscv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuyxnjng.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3rteexprp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3oekuthsr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fmmhnuur.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3dbwdhjjv.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dnqdyzwc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3lrcpdvgj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ztbugouu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jgzwkirn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ctrryivp.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3kwmrsrrj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3gxrqvgnf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lmuugjwr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mitmlzjh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ayawpcxv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3srqhfnea.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hpzpxrax.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3azfpbyhi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ghyvayyh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yuurubue.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ldiohcqe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjyekxpa.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3updtdiwh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyqyhhvr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xvmoswep.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3egqfwoxf.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kxpalplg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3llpihtcd.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tmbqevvj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3zkonjjao.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ojdqsjip.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3slaomnbp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kvzmzzil.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xwxeqdjo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3euxymhld.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3zxpzuxlv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3tulxuitp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3guimpesg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ydupptft.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3cqetxszi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3pfajxvyd.html


<!-- 参考信息 -->