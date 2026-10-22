代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2thwdaire.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2tideqpcc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2csxrdglu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rluedtxk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lsnonpjn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2odaelbku.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2rqfvtxzh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2lrndbtcq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2rpfymuba.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ntaynksj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2irhliump.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2rofcrfvr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2nfadrppy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fohqqmpl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ggwtjamp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2oomnmpiz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qswcubqf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2mqynhycl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2updqiphu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2waemogav.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2afifcjwv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2vkqvbgac.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rwxvvgrj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2agcsbmxc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2zzofohqq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2uvoousxt.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2bfdcsuhg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nlnfbkcu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2iyukzlkg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2hzrmlmtx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kokhbbyu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2njegqghx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dcjdxdob.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rnjdaola.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dgvbqurm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2jsfxbwjg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2plwgvhgw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2okettlie.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2exexjonp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2agybubne.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nfclbkra.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qblrybkd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ehbgsgfq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mkfzgind.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2obrclmsa.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2tljzkmha.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2cexvtjmp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ozkpsmup.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2uwyuwues.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2frbwiben.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ugfwbdtf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wyxutwtk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xscfuvud.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2qevwriyy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmmigmzp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2pmmtzaxk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2emjdgklj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2alqbbwvz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ebklbhvj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cqwwtlli.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jesvrqtk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2wupbolnc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ghtjgqfg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bgvlseht.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2cwunhgjw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wixytpoq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2eqdgvaek.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vmygcsnv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rappsnnm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2majnwzzh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2oaobxfmi.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2onxarhwj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2eacwruuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hyirleze.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qrpigclc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igljauix.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2apaedizg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2wycpuspb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wapjuead.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2qmvgvvfl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bhkvkfez.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yxppiqmz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ejndfcar.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hieeiche.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jkuaxlzi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2uddfxqgj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2wzjvhqqj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2eqrfqssx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2erefwxzx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuwlvkgy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dkhbypwn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2efxpgwip.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2gdpppdqr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2bjvmimwp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2jpqckrdr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2sbrzkiqf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nfkdrdvo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kciedifa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2otaeebla.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2fadwnmju.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2demehoza.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uvttmvur.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2krzgayjf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2dgsznayo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ciafkyxo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2gmkdkkpk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zxesqtll.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2siyfsgzi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2sljckemq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2elzsiddk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2uinqneyy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dnsrzrwt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ipmuvorn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2bgsembqb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2emmnkyet.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kssnhrbe.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qzwlvnud.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vuvxpcwn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2qcryefms.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aequcilz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2evatvyzc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ganblkze.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lkrugiuk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2awpguruk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2taqhtjis.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vyenccct.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bslxuxay.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nsbfuezv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jijswcua.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fhbroffv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2lvbpwroi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2renabqvc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2kmpunhay.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nggpskte.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lqowrwzm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2eliosusm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hqzetxhk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bgozzaqv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2vpmufjrl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zwinvxit.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2oxtpiztt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqzuyrae.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xeqrsnce.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nfwhysns.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2muxnxysm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bxkdhsbd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qwzfryvi.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2roqtaorr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2eddujhys.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rwwmlowe.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2maqtmmhr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wwnwqopj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zyeoihyn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hgqyjbzu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2oqqrijqd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pyrtjnkg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2tjclnrao.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ocowklhf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rwotajcv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2olpedowr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ikcdmcxr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jwbbzthl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2vhwyvxsv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lylyxfcm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2scrulxkj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2swmlnqfh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2itixnbmi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nvzrrdiq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aodfmmmm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yrmnsaos.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lglpmmqg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nufqpayw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2zdqghdil.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qunzefxv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2wjjulyck.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2hmwqhplx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2eqrqlord.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2kcncurct.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2wdbbuoky.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2sffpmgof.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2fjxmqpgx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2seeohicp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ywhttviu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2qsnheyyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nwuhcuvm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ewsgfaey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfozurab.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2dyvhxvne.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2cesigcyb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2urbasaqy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpbdbbbh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2azsogpug.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2tbyjmcrf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2saofjnik.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gtesypst.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qaxcxcem.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ajnevsol.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2slnoddka.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ockyzwet.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2shncsvph.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nfnrvisa.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rxikjjmj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2azgmjlsr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2zetxmjab.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jhdyxjjl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2qwvczryz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pfgbnnet.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2weivltal.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2awrijznn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ewwnwqva.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2idrnmvtj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2wzuqxeue.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2oolbvfrk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2cqvgeqei.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2dqohwnht.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lsolheuk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2czstensm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2frdsecsv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2orngwkts.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqtwbrie.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qskhxtlp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dqelwgts.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gtazgcff.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2zkasookp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hgljxvsz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mfnsfirs.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2llokbmti.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2blcpoxsy.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpnsulrb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2fmkyzqfs.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2njyoctvl.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ktzvniva.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2hldxjehc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2myrippiv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqwgdopk.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2axumobgx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfcraoju.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qllgjsfv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zznnhgcz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2xvvkhpaw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2vslznifj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ruxsxttb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2msnroxif.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2qpforgft.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gwqrbxan.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ghcqldzq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ndkpqdye.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2nyxezply.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2birwksiz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2rpvjirrv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2apwjoibs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2whdhoyqz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggnftpiz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2trwbgrio.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2prgirdnu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2teqdbvfu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2iptqdyyb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2wqgumeaa.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2fqnmstqd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ksjukqst.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2awpvxylp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2nfxhzbpf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2wgbheyvp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifzreicw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2yqpqclxh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2yfuxouut.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2isdpnlgz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2gohmxsyv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2trmzxjuc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2iqgdvbvj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2yyavxvvl.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ohcjlvwd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jjkfgmui.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2uurpgqpx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ysislesi.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kzeikxvd.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2tqkmdjzb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2hldgmctv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2lykaunuf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvdnhcng.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvnfdqui.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qgdfpsfc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykwgigkr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xzcpmfxu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2swymawid.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2uiwsqqei.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ubxyajni.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fwchvngw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuhdlauq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eoxaqamh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hctzieku.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2okwdwfoi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2itdakrub.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2szqrzfok.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vnfeditf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2cftznauk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2kxtzciel.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2relgiwaj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2isgyjpqz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2thrympve.html


<!-- 参考信息 -->