代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xsxudnow.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3kolbiqai.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mexghzyg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3qrccsocd.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3helvwvyv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3iyswylfi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gkzultdj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bukrxfjr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3bqegffyz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3wvxxnmet.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3uvxadyhl.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ciheembl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3lxacenkz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wrckqqpv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tlvimlim.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cmwwfppt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3rtpfbwnx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3dnlavpdh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3znblsieu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ugatydfs.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3xxtnbwdv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ovyhktps.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3rgjnyxly.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3azrivfoq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3onkzdjgi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eiytrgei.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3prbttidr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3siaeufgw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3qwexnqaq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3cjokneof.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3odimudwr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bcmgvoyn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3igtzaerv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rpaotyjt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3xxzqwxcc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3dwvyvuas.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3hzdbuecm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3aipfyqus.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3enzmzjuk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3uqiuykwv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rhtnzgkw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvpamwdk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3uaafqhfm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3uldjraes.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3afqmixgm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3kjutpats.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3xmszxyyd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3kymaerzb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3iwdjikfs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vmibmadw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ieqrlthx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3smaytsgc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uhhfqcqs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ggauprau.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3whheotof.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3umzjhger.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rrrqpkea.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pzfgpnxv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mofmisal.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3txmcwvas.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ofaizegj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kebkvbhx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ftnjhnkh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mwzhgfgs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3iichvzop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gpjsufwz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3vaowfkgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrpedpmj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fwqfgdrp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3dpbmuipo.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tikdcexs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3itykyixm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3khpprbrn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dpluafnn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3wxxfdkuk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3awlycnsj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hwcmvzrq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3cphwhdna.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3sfhoiujz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3hilnbcnj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3arwqxtgj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qovbksda.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ewmucopc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3jqihijwm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3dalmgaae.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3efsivzow.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3gbwfgrfo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ukrmpmvt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3edbqcfcn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ceozywhv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ubqhnttm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3fzwxcwzc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3sffcstar.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qkrbbehr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3syuunllw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3uvwuikfy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gkcycxrv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3qsvbvbvu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pqvjcvsr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fntbykgk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3doeyxypa.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rfigxcdr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3lusgvijg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3jhvnjatx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3cmohupoo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3sptlcrwa.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sffjedkh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dfjsdwkt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jmarlozo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kmnwjtcc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wkqjfuqj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nwjdfgbi.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fnpbtdpk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3unsprmwx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zobknedr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vxwxbops.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qtedhjkb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nkjluqmx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3psahdgqv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vliszskk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ojbtymqe.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zhgshrmr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3toeltrha.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ckazoqol.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dyxnuhtt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3johhbnhe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3deuietlv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3miznhumi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3uqawbsbb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3zwiibtqi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3uiwuuvco.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3cnksovqt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3fsbkjpsu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3yfitpgqj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3owmuosmf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jephgfez.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tfxydvvr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ghfcgyfc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tcsivtpa.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3pfigiljp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ownrpyys.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3caxzxsie.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iczzeyth.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tzfvijzt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mqdrloay.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qdteaenf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vnrrptkd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jkvfbyvl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3aimkcsfy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xolnddsy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lwytawwn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3swoausuv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wtdhguqq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vwyvgyav.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3iacanzvw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3esifywle.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rklrekrd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mmujnnxi.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3bxjndbwv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nvmarpve.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tehdcius.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gqxvpwyf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dbysvfsp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qwmpmoew.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3crognfyn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jhjkofit.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3wikueoay.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3hajpuufy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qdddecxq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3rulqrbst.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3hcxoopqx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3rzsytjsp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3smwswilb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3qsvtoqzl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3qwwdsbxb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3tgpfsnuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3caehqigy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3wvlmhpjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdulzxja.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3dbyqwlnl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3xpmqnyic.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wbkkbkom.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fyipiiun.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfvjafxa.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntysgttk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3yaunedyz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wbnvfwia.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3czfwbgzf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3wvtnsafp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3namuhbft.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3fhonqzbo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ujfqkecd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gggewtrm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3boiswccz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3rbxycubb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3luhqchwb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzmnpllh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3pdjhsyrk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3favuaiuc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cybwahfr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zmsbfmul.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3enfcphnp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3wwfsgqpt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3faxuiedg.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vzabgkmk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3jghecvju.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3sarrguvv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dqinbtwn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sktiulyy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpejrgdi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbrbsjtr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3itwljzgq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yqwhgfcv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jaksvqhg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mieryqod.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3rvyrufwa.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hcvdbioq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3psmzmexj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uuksvxna.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dftxmtul.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uogigqpw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3txugtgvx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fralmjeg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vywxrfdx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3igluxjqz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3xsxccimw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3leeffjzy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ciifaloc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmgtszzq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3emucivnn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3mhvfsipc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ctnxjjec.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ehoiawtp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3tnwxqbeu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3seguzxsq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vwfglpwe.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fqsdjqke.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gzjxpjos.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fmssbroq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3gedintrc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3nbazhuvs.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3svshnwyc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3oesedstl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3lfskvdmx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbjbzers.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3czehbmuz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3tzicmnup.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hyhhaxjr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3gjaydsuy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3uxjofsfg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3tbvamvig.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3qedwknmm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3qrenkzpe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3trsiwzrf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3pvjnbftt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ipipcick.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ojxwqarn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3eanoyrys.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3itwquigz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjqayyia.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ooaylkft.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3okragbob.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xpkfcbdz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3culwlsxj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3djykuwhu.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3tngkstrf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3bmvjpnfa.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gfkuvrky.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3jogjxmym.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ugjkgxnc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3zzhiechm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3npjzszql.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qcomyejs.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bmakxaop.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3btvfhaev.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mppvwtbu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ytbdvbqs.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ydnmjvkb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3igidxauk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3omlklcqn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqwzcuxc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dxfvoznn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qmkpelth.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vjbqxoow.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xdatmody.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ktcmxeqb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3yrevgjxl.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ztxxsioz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3tivmntng.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3snmswaeu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hxihmbac.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tyjwathk.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xiqbenik.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3cfuubsss.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3chiomegz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3bwkdzomb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3byogieqw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ogwpiqqu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3lvfsxjqa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3mfrodlqw.html


<!-- 参考信息 -->