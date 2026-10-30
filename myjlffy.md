代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gnmyhvnwj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/giuvijjfb.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gkqfnfyod.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gpmlkrsph.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/guvqwgfwk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gahryoopw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gbdmtkmeb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gqyiqqvdw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gjagwahsb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gcmurazsd.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gdezepdir.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gojmpufsl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gasupowpr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/ghamaqxvh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grjurlcsp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcsosqkwj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdhoatufx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gdewvbnju.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gebftunbn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gddoneduu.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gzeiwqwfp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gwqkgeoek.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gimxpxinr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gzvitupcu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gsnylmcpx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gnsbcsjfq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gbuuuwzrw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/ggzlwjyut.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gzpxjuddo.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gfsdvysjt.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gtbiigmpx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghvwlojqm.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gsoyrxpbf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gedvpwvqs.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gpqkidxaw.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gocypqrdp.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/glrdvupyz.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/ghvcfcfts.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gsizvujic.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/glzdpripi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gajdmuhow.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gpnmjjtuw.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gyoinjxpn.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gegpdnqas.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gbftjrczl.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gvbdchrbu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gyaohfril.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gczmhapyn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gozkxgejz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gfnqqxaqw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gjtotklll.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gwiuekyqd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gbcroybop.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gscftlbux.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/grfkbrazn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gtvrmaoju.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gjudmqwtq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grxtpwpox.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gjsazfnnq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gtczeufjr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gsmwqmzck.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gecryjnoq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gcvnlgunb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/glqlqdtzv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gfzenqsxw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtehqniml.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gvbrhwrrx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giwpgggkb.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gnbilrjtp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/guuydmcri.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnrlantjv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/geyqvlepb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/golaplwpn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/ggiltqbye.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/ghnbwtuaz.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gljnghesi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/grpdjgeft.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gybeodirr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gghoopfua.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gllzjtzfq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghetgroii.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gcdajetcl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gmyuywklv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gaqeviukh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gbbpopesk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gxhoiirut.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gtjbuwnxr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gsqhoprdz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gkwamhazv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gcoaunepd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gtnsjdipb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gblxnmndb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gmsxdiyon.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gyccwyrrp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gmroeqpey.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gddhsdxle.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gslnfkgfy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gkrkxwmab.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gsvwftmrz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gfgzvcdgs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gdvhkykxj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gzlpbtreg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/grxbfeymm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gzuijrwin.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/geewtrmgu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gfgktglbs.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwmwolblp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gskmbrbey.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfuumkbpk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gajysnxex.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/geyqpjxqg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtzxxwkvk.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/guhzujbye.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gmwyqxenq.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gosrgtrsm.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gbllemobh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/glrfaieny.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gnzvpgdtr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gsxzvhhwj.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjnmcqgci.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gykuajyyy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gguvujklp.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gzjqlxnha.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gqwzblras.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gzkptxcmf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gozqogwps.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gzrkmghkc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gxjnscdbe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gsupunakl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gnjayzwbq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gkihshshr.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gtastgfct.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gxjdbbles.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gtkghnzdo.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gkxfwjupf.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gmybsvedw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/glnkyzmtf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/grboqtghi.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/giwnogqyj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/ghgfxgdjr.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/glubwafyy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwperwelm.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gutspnpzt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gthdhxxmx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gbcflswvi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gddpobdos.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gmoanqufn.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqymodjxe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/girywmpaz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gpdvjwtbi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/genuxbnxo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gkrqwvwde.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghqftovht.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/ggawpekte.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gshzfpwyw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gafdgwsua.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guqaqlffg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ggticafgg.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gxdtkoepp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gugzgzozx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gzmboszyn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/grqasieah.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/geewjdjsn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gkkiebjce.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gnbchhzld.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gvznqylwy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gkhimahje.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gmnytwcrh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gjqwqsuel.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/geninfald.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gohqcicfd.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gjzuwfupi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gyhmyjbvu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gllszggpz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gajownbdl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gyztfxcmh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkmfsfpxa.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/ggsyhljkk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gesmajhuz.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gliaxdfbg.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gvgwyrvmr.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gmqkhlgek.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gypahyota.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gsqgvgmkk.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gelotjojg.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gquxxoyav.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gmnqhnixd.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/ggqgwsxgk.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/glxdtsisr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gggzpnuzm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gcdvemeve.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gasjzwddm.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvdiuanih.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gumuwkjmd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gyojgslcq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gxkpvejwu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gznlvscxc.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gpakidijq.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gtogfddpm.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gqjfkltzb.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/glikzheqb.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gviyvysan.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gnoxbszei.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gyobqqsng.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/ggunjkmle.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gmugfmxth.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gziwiwhei.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gwsxrmzeb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqrhdlrja.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/goetprujz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gahkzfbhz.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gcydqqspm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/glataugov.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gqgnujshs.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gfynhaxit.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gzorfgdfw.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gpfyynwnp.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gdvanhrgb.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gdpsvhrql.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gyzmmlgfg.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gtnhimcpn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/ggsvkmhml.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gsgowxlkv.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gmnkbfxzd.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gulcgjbqs.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gjfryyfls.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gaansugou.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gakkeftyp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/ggmxtjnpb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvkvgene.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/ghznhgyon.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gsosdnylo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gpdbkvvcc.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/grummgruw.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gjrzslhqr.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/giwbzzhgg.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gdrkmijjg.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gpommhqjb.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gogxmwehz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gfymncprc.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gobbdxzwa.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gqupspgsi.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/glidrkkwf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gcceqxrcn.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gonwmizxz.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gqcgmxeor.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gbgmwkfwh.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gdozmhkct.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/ggysuzkly.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gkzbifllv.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/ggcdcuugq.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gwznbgcwn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gjhfcfete.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/guscahjlj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gajxkzlje.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gllmvxxuq.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gvnesfpwl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gswpfhhhh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gfjolfarn.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/goqimjlaq.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gtervmtou.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gcjoeohrv.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gukxuxsry.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/grkrcysje.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/glygeortc.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gjwubfvvl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gxsnjkqrp.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gusslbjoy.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/ghgkzvasb.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gzjmrbpvt.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gyzuauvij.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/ggvhtacvy.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gyfuvratw.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gjqqxflho.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gylqelmko.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gdrazymwf.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gnnspfeuq.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gtbxqaewi.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gisultifa.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gamycjytz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gvafxmcml.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gqtwyqrjp.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gtnnbpete.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gcauzekgg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/guzfwojss.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gagmtpcfr.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gdbduwvfp.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gdwqjxeym.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gzzzyssvf.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gdtoiitcq.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gggejlqqh.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gubdozdxi.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gcwchvfzk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/ghtgdumod.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/goofpyzes.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gyafpmodg.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/grspebyhm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gxpgwosjl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gqhanfdgp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gpjalpmks.sHtML


<!-- 参考信息 -->