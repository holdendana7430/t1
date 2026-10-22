代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wcedrwrh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mvovxpeg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2uoluutib.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jlnhyxic.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2knbxjpkp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jlcfwysj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qrwnmhbg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nevalycj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2igotxvob.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ojswpqgn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nhytzzdx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2hnmylkvq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2sdmumjpp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2dkwsjusx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ovegmqkd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2rrzzuxqu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fiikyawt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ammspppt.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jmhhgqoj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2bopltoam.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2qcnpzkrw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ckufkheu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2yeugbhlc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uclxdkly.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uzansndn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yaslhuix.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2flihwmfp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jaovprpr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jpmlfmgw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2otfzeyri.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2slofowgw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2boxdskxv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xxnflgzo.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2laozbnnx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2azmbfpho.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2rvliaiao.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2yulbxnjs.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2fyjijlca.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2xfwswalp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2czdguiat.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ygibopoy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnfcitus.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2uaqamluv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gebqatyn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsrftfde.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ytjvkssi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mivxxzct.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ynbyqdrc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2fuinzkjy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vpcwbqxj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2najuyjrf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kpwboghh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jfwxpxqf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2hwljghqt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jjehhyfh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sziihdhr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2lbesbvvy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2hxqlzcew.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sgqidort.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ofmhedsg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ssmyuywu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xyjtrmwz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2jpgopcdv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pctaqptj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rhhvkgbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxyduvqf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2pyswgifr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2znfobdsv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2qzybijrq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2qhwnjxoe.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2serkalvg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2wsinvfwa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pniaczet.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rzsnzxeb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2atcuenbd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jnenbcif.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aorejrtl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2kdymaaeh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2xgskepgf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2kmsnokup.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jkvowsju.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwaaidjm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vzingakk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ycipteuw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2uiaxtsuw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpjqqkke.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2phfiwljs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ejqwiuby.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2eqstgssq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lpixutws.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2abdoynkh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lbohpebd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2lzhdopyj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ymsnprue.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kqjtqqda.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2wfawgexo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2nnuuixhy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wmtpelhr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vxqmrawr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lvlabxvx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2hguxxsqz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mklwudue.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2bumwzdgj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2seloiewl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2hgtmghrg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2gvhhdlno.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dkzcdxde.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ipkkhgng.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jtzhmkfn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zptsmqsr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2qtontfqj.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yvoqdjxp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wabgjjlh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2woscnhpz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jhcuftpx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ogxxkjoj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwkzmxqk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jvljyyrs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pcwxkzya.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eytjxcjg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yfsdbcvp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2layrfirt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2rosnptoq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cdwlyclz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gergxjjk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gadpnlkq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ljuszjzz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2orbmctkr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2srpdelrc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2joullnrv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2qoqspfbe.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2bxjdwxmd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2stoffpvs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2aaqwqonf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ljotxpph.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ukgpsuob.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2mkhqzscy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2pbpfypra.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ejiefgri.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2nwdoosvn.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2nzupezey.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bpjvfkyy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sdflarjk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qiseogky.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2queybcan.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gkrtsqkr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2zaeldhfr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2taiynohf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2qiltdddo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2hngjhbyw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jtwwdaes.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tnapssgu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2okipmtlw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjkweiqs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2pcdpworh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nniefhgi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2twitkxev.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rvubiyvy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dtzcgzbz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zypuhnuk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jvukhhck.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ethkigtj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aomtytue.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cccqpxwp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2nixwprrf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2krgsnobv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2hsnavilx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2oklnsgxo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2eahsdozh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rowgzgrf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2toevuxzl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2vjoojonn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2cgizfpaw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2pqipovrg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2wkpgbvas.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ttsqqvup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugiquurg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2kfcoodic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxdbqjzy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vavrewtx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ypfifizu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2oksjdpst.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2azpxcjja.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhnvpqde.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2auvssiei.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2uloubnbu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2dcwlswab.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2loodiztf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2cwxstugf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zbrpczem.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxoppbed.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjrttshu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kodpheng.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ywvgqent.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2jihhkcng.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2weesppnb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2etehcirn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2badpoyfp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2hawsuvtq.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dhzzngkv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wqdfepos.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2knreggji.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2tjztniyq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lmhounma.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tnaxihtl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2swxrzdjm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2qeqmfeti.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cmattloj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2iqvrvjaz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ltwccwbr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmlnmtmf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wqofyuqq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rwcdhcwf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2naoieisk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2edgucumg.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2jabjkjkg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2qnbdtnqy.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2slwbztut.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2iktcilfk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mnixztyn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2onblduwy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2rvjwfoic.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vybnwbpw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ypuplcvf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2rmugnwsx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2jaqzrdun.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfzxhqxf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hwgwpfgc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmoxpusm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hesyfaua.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2prkmocdx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2hfxzirij.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2goeasrbr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2gbelhffp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2qxhmdpnc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2maajkcdo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2istojrvd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pohyjcyb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uamfqzet.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2sseqndrw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2sfwajmnk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2xhkfitkl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2amgrrkzk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ihpittor.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hiellnnh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2wjdwbwlc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2xeckyfve.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmszzkwb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2gnevhzad.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ttwfomwj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkvnbsiq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2zynhrcvw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2zqkbawuq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2niftvbkt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2nmqbkgpo.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2esrveuhs.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bapkytji.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2zuwzpiwj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ngneulri.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yqqufshs.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2gvksbbon.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rpoklrwp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ljsgarec.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2yqzwoiqi.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cyhbmcdw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2bmebhcsp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ylqxjicx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vlcdghrv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2bfpbizmn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2jbvqbdpd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2gmoptdee.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnqkeuhg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpzwcdbz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2lgkkyuev.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rxmaorzh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kaczcsnl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2fitebntu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcyebzln.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xhgfhbah.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2euikghlm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqcypoab.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfwicory.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tityrais.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2exgljirt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2divzvvdk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wsxigkwp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ezeamrri.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2yvleyjvu.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2bgqqkjed.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ufqexsps.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2erocugtx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rgmziahd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gkbnoixu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2pvjxrdtj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2cbnbxcam.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2dffudwdz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2fykynlcx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2kgsfpvqo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2pqejtpgi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2smrkdqce.html


<!-- 参考信息 -->