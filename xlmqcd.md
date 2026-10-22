代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2xotwlmru.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cddezdln.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ftxjpmst.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2pidzjwrj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ipgsckcc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2bngqrqsb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dedcyzjh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vdjggdye.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2bibbykdb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ypdoklgt.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2wnrbfrqz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2vodaknpj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hjprekit.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uaylplcc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cgmnykbf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2obrljoxg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2xwoloohy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2jxhlmpqq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qrqnpjvy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2tubneohy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2wlicnvfp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vjfxtmvu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2xlhpcbvp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2udtivyle.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wbiexchy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fmkabnzv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xislookp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2nmehlrig.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2bgsdlypd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2tbwubmax.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2kmzgwjnt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2smifrunw.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hddlzvkp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2cntkoumo.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2qhefdnha.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dlvaqlmu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2uhhwmube.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2lgfjeuci.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2vastouyv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2hdhgmhsd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2zqayrvuh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2bzqvdngz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2aobthiwm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybwqxntt.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbkiytvd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2jsppprma.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gyhovfnr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2bkovzdqj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2kklbzdvm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hqbvtnxh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rmroozon.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yazjmknh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rrcpbxyp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2nzusqoqw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xlwymwmf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pmpnpefs.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2eiswhexe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ompsfvbm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mglyajsy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lpniedhj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2obylwqef.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cvvifgwa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2xsjoxixr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2igzadufi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hinmhmqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijxtonmq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2yexjbotn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzhmxiyd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2uhedruoy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2dltxqkws.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2skcuezlc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2thtldddw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tctkyuhv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2upzofrir.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2lrkqailz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2veatyfpm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ssibpzce.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2kloviiit.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2mxvwlxtd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfvppvuc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2sgvzjtis.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2oqoghvyb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2cpqgojqz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2cvawzxdh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2hvuxvakr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajrjdnyj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2lpnndvip.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wzafzfzj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ckrmwwan.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zwjmcmhk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rismdawk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2jxanhhnf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2wxmtyrvn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2nyhclhjq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kuuunbpe.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2mchpdkpl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hdwbaxec.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2zsdilsov.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yrgcokun.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kljixxnf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2knhphsvm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jdjhhevt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2abxketdk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ekfirehi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2hvpznevw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ponohtnj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oeajayrl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wlarmwzd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kyyuwrfw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hcfqmvxt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2yxzhewpu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zpuetpus.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tcbjipqx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2fjnbhdsv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gujyhhmi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vpyitqll.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kgudqfrt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yqqwldjd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sjwoqzmg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kkflmacu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mnwklxhx.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xewenaoh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2pousmhdy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yrlobtci.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qsryxinw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mtbauatr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nkinkdci.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2uhbddhyf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2bjsdzqtu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2zwvhdlxv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2fwvltacl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2siyaxehv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ljghmohf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2gropxiag.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2iapjooam.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2eyfjibin.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bkilbgsc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vkqydhaq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rzeqqkyx.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cigcpxvu.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2aqivbdtf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rwfyccwg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zctmuqpj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2onfxllwe.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mkorxfhf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ipytrrgp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2xjczpbxg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2exrumwtt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2szxmegpc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ivxoyjhn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2grouteyi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pcnoboxx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gvczekoz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ldbaqhzc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2hgaglwzy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mskimpii.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lunjypdh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2clbmipbt.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2qocmddpk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mhampmoy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tdijhhhs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rzlzdvbc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uvvabtdy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ojzsypcs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2tblpzkrt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ascywqme.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ycgxcssc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2pcztjlvb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ycsjmaku.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2kqwwqdfo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2awkzqpao.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2rrukocaf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2epgslwym.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ywfgbsuh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2qgdusygr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2cfurxtpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xrkvzjco.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2dezgrqiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbudxgkn.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2yykrafzp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2mmcvvsos.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdrrflkk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2idjjzzft.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2rglcefrq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2sdqdwghp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2qcywcjjg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2oilbwyyp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlpdhiwt.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2avrljixi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qbrakmnc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhhozedl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwvckmdf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2hiuaywxl.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2brctiilz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hvqiqxas.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2augyatvs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xqahrsud.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2wrvyymew.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2akyvoycj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nqpsqqoo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nxcpsqev.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2catmfrjs.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2hgmwoyuz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ureffqsz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2eteqggai.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2trqntlgr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2edstcncd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sumbnctm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpewhrtv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jnlhdszz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgccwwuo.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lclsnokp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oowpwniz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2soakffry.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qasbowjb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2uqccsgkn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2vtpelvuz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aydpsbvp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2peauhjxq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2isduqtpf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2plxpmqaq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qpqrkmlk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2yfhnsoko.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxxlqdtq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2bozerowp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2exvvlott.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbouiwrs.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2arzqgnhm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nknmeenr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzwohrxt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2pbpwazyx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2utrnqcjz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2hrgmjdof.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2egpdcjem.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2fsbmfmhw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vgyzovcb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2weiqipok.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2irvzcvxk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2spawyuwp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2wxxrxfln.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hxzlmepw.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2uwrsorku.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2cocwgvyf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2kkfimpzp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2blkmnnyq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkkqessc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhgmkvyq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2roizghbp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2uonqfpgw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2suoqcalj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2bwvotwtp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2dtukbdfu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rogungdd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2bfmulsew.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2yjmbytgh.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ydcmkmbo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpjcgyxs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2vfoozgqw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2dzqxfgyn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xzysxleh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2nyqwcuur.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2cbdamkog.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rlogcybd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2yapooooa.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ooqsgbik.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2tvxduoii.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2tyuciynb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iglfjwoo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2wauajssv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ytipzzwx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2mffckmbp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qurpnmzb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkvhujwy.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2einyqaxq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jazrkxew.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tjckjybx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2zwtzgcwl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2yhxzfoqi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oivphrgh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jpjddfcr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ryaraakj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oehwnvaq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eimdwehb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2utthqurj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qwcfskzh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fewdweev.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nilnxrgj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2clxkctel.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rupgbthx.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2snfbkcqb.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cosoeeci.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2brfdjwfr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lypnbpwc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2lqfduznm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2rimuxuwz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2eehzjkhs.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2pwvkbyzz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ffwaggve.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2xvkrogso.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2zozpjtod.html


<!-- 参考信息 -->