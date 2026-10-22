代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bucrcekc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2zzjjnopx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hkbvtqsv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2popyreua.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ecitlohp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cdnkfvjq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2fdifiqdc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2syttxrzm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2tbpdccuk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pimgdqvz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vpvenfxz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ippejyqs.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ivgwicpz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ibavtmug.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fuxcxnyd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xayicpkf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ybgxqoha.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rjrxuomh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2mxjliilm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2dloonjtb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2gduiilod.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2oqcrxgmr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lhvvjpjx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2higfrkpy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ihyvyhje.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2arjjxnxh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dnjrmubq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2jlfapyak.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2qcotrevv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2mgpzhikb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ixthfesn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zjzvcujm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2syuvdkbu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2putlnnqh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2krdjsljm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2rafbtxxt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2asatbzke.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bpychkii.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2jzmgjsoq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pxxpnjcv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tdwielpc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zhenztjn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eoysujxq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uodgleyc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zjxkywqp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2iltkfclg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2scsxcwvt.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2bfabllgm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2kqfcuffl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qbqvsqxj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2mgbjfife.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvmenewb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2zhhgrznl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2nehmtdmc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhddegpe.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2zgtuixee.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2bueozcav.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2aadgufbt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ikyenvdm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pyxjzqbt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nhiogdtz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ulhntpaa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cwpteiyb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tpbltbli.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2uegtwyjb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2dljocjjf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ycqhzwej.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2crpcpccx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ntotslwd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xkizburf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2udpnilbe.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ndlpyuvb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2izbfxrjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xytscgab.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2rvnrivtx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zkgwrwwp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2nsmzeknu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2vxjwzbsk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cubcucwn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2xoedaeeg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vihmsuyy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jxecjswi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ugtmqsqn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2orsnjdfp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vwzebnxq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2jykwgxkl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2dhzpglqm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2mtonlyyr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdpzqasj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ouashqkr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cveqnjak.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2dlkwezqe.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2phcrcjwv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ebqczcbl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2gltvdbrp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gxiacozf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2edbxlxkt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ivccbluu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bzjpmrzf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nvlgzezx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2uoqilztz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dzhmihli.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2tkxicwtv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zxowwemg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2bzkaukwz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2jpdouwuo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ruacmnyz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uystlmmc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2qydaytqw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ukccshbi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2pnyigfdm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pjekducs.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2fgejcprn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2oqvxrxbv.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sstjnpqq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dcrcbyym.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cqxrsbbh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2khhpkglf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2czohzioa.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pwmuzldw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hcghtjko.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2vikotvct.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rhhizvai.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ujjfuskd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ukzbewaj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yauitjcp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2oanqrufw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kghnvzgb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rwhbzhrm.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dloxcvbo.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2adnktvbl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kpfwghgi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cfsgvnhc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zfjhzeru.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vebihrng.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fbrsgjjk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2drogfdwt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2vzsuzzig.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2nklktziu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ccyqhdlh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2kbhwyuav.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkdsilvs.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mtvymvdl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mtrobxdt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kjdpvnem.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2hdsjemdb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2zpufzoic.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2vgehnvwb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2aqrvdjsw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pvcctdzr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sydxjina.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2yzljxpbv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jvqpftnb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2akcgnoke.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2pqzkjhjh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2skgdldmf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2dmyamlwr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2fjwwfljh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gekcoieo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qzzerqse.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xrnqrwim.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gzusclcn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2hibwdjyb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fssodgie.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ejlejafq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2waneqzid.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2tarkgybk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iebjxitp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2windchps.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rudbpcfo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2exirjthh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wxorcsrb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2bbzunscd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ywdrofir.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2kcpvwuuw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2bipjgnkx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2hskmwewi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2yybignam.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2hjazvvje.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jgedtwca.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2emklmijb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2brimsaak.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2viyorlbs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2xbjgfzez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwptzhbu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zerligek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhktyfvq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2wocffpqn.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2euvdvddd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ssyyglfm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rrfbndnu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2uyinnpfw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucyqmolj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ryzhnmjs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2qknqgwkj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ajppecac.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2mncxscxs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2uurwjrfz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2gudygudz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhoxjfwu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ujfybnej.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vareoaif.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2phahldsx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kubtovla.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyaoocme.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2uelwveqe.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2askfthza.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2scoiklrj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wkfxnbog.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2amqaoaam.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2xmhnsjxs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2gyarpphd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hobslmxw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2vwprlbnd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2gojqjlgy.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ajqchroh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qfmrdpgi.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hewolmzj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yjsjyyai.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fdhogawh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ohopwzmj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2eceqavmo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ujjcmsaf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2fjfdmqdm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2uyidffcr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gszvjeau.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ycdtmsbh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aroockhy.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2daqndhtg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2nfbowgya.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2uwtajtxq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2qsnhpjtv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2brdynuwi.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2sasvuczy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkcsyrqz.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kotbgqga.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uloubmwl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2njzyebbx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2lzszjdog.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2qfnoeoch.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2jcqbwhor.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2clyaqxwl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2iomzufmm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vbhzelrd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zfcudzqu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gbpdtpvx.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2spbkhhiu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2hnnxrjcl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hikkpqkg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pzgekgfo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ciexvwfy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ozscnqst.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2maxbhbit.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcligteh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktcajdoi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxqozhse.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2gxpqjcny.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2getrqsjl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2zworknfe.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hnxlrtle.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2yxpfxpwg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2wbqxgdfk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2xheppqvd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2hezaszfb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2kbnbjtvm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2itjqrtqc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2turiwyzu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wskxruup.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2uwqkxoyq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dguvyzmp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kyvcpwzp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2nwlanuau.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dmkvjgoi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2lxshvipb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2qqlnxmtq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2eummicsj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2abvjjshl.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2njjypycw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2tquqlijq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcucadqk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2abonqqkt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdpiawtc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkvhlato.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vhorvojd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2oqgerqey.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2hudzqucp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ivglylfj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2pbovsdsm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujusgqjb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dpgwqhet.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzgsmtag.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wxgfhtin.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cbtvzjqy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hkookoqz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2htcdkbvm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2bmwinley.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2teayfxnk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2osehhsgv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yuxvxrzv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2huhegjif.html


<!-- 参考信息 -->