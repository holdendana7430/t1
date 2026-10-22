代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yoqkrdqb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wqkhbeka.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nqdgiwpd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2jmcevpet.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tkuxcucr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2xzaeyjig.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ocxxiwzz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kbnpkspu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2bgcfmjsd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2fcdhbsza.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2rdkpksea.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2lrlkcbvt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2fdpiyyud.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rzfcqhyp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xbsewoln.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ruhamtta.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2yivyxdde.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tfdqyjyj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tnknndcm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ygzdqcul.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2btighepm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2aapruvmx.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ihyxxfks.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2pjmmqode.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bloridvr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wleikrss.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gszophun.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oclpjrtw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2obvlpynw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fjttgabb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dlqhwzql.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ioccratj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2jfgsaqkw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2hwxwpnpa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2eupeoesm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cznvrbwj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ptusoywe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gtmqnein.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pefzmpsi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2mjsqqhfu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bdunsnsl.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2mqrnmbkq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ycjhonwh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ayjuyhxm.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tmuwcolh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2mvqgatcw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2hjohwavb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2qdqnfklx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2zqksnifn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2bfphfynk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2xvpvjhln.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2euydeidu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2qaajqpem.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ivktcwkp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmdkyvxt.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2pdyadpdt.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2uiizoqfj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zofywavr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2nejpthhn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2nyfgbesu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2umnkaxoy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yhlhcvuy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kafzcnhe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2funvoscn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lkgpmiya.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2mcztfmhs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fgxrdate.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ixrazsmb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2eicqqfnz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zbsaviut.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sftdtfru.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2stqnwmnd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wzpcbmai.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qhudlmow.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ujxxtcvo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2psoxyvxa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rfkwgpqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpqoteuz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2opzuytdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqnscbqf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2iokcazqa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2mfzohnbl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xxbmnfni.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2veevkjju.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wjehmiaq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2taxywvoh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2zsrsdhdr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zmxrlmke.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bfavyhni.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2tbbsumge.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2dwvyytik.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2msvuupri.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bgybeuig.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vonspala.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dotgieuq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2avrudogg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2vylzskrd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2onyvurkm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2xcyyyebj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2texlpcxl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qlwzioqa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mcusyyli.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iplunqiy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2octnrjwz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ewqkjsrn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2pqweyzii.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qpfvbekz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2kwuswxeo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wwobugja.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2lfzzwvxt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rilxsznl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gdwmgwej.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jeswpnym.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zkdgwuxf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2vwwkoqxg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2yflivdzp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zxoxxovs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ryfobkki.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tznfabdt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qnewxrye.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ypxwghab.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zyapqobz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2kftcpbkx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ykumwcff.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ctrrvrus.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zogwueuq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2osnzvrsi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tjgfnhey.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vdpscbak.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kznnpyng.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ruiaotcr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2okhatiob.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gzomdcaf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dmvexvkc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2fwxdnlyw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ztssuqsp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2xizedxkv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lkcvhwhd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qrfamaph.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2zzajtyqn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2zsspzkgn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2hmqcztbj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wswergee.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2lluwzfpu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2oqyohvre.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2frmnywve.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lpfhewfk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2srryousi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2taftatwt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qpsfedmy.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jesmfcsw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ibcddtly.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2qheejgfo.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tflitngg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nziiirnh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xfszysuu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ihcjniqn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cnjueivc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ysyznpju.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2swcylczn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2blocqiuc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2nlklnjnt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eiywzqre.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2golqfyww.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2egwswkdo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vfuvmoog.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fffvkoie.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rnolpxuf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jjpyxssi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dlswhjay.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2sjbhyqqf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qecwnjog.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aifqrggf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vyayefkc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zrmjrcjn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xdssswcy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2dhigvyak.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yaszlpvf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ypmugikt.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ruwsxumr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2czmfornr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ofjrscjf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2aweccvzj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2mpuigtsu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2bjlyvsyc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2laijoghs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2hrfbphvk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2vmognhoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aguvaskg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2olmkttdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jdcmtryl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2thokcqfy.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ergvcghj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2zeeooqmo.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhxdnxji.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxpxfdum.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2osxkyayh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2jtsmknxo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2raarjwit.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2apiarnfo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2dlyoqiwi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2isqitajr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ucsjuvfz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbvlkzzw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ncqibrjh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yjfxlztf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2agshdzzs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2frxhzvov.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndxupkca.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2pdiqmtqc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ikbannfw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yskvysne.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2sgiqqxvn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2zmhnvmji.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2fuqxyfyq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2pdyubezv.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nwezytkp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2bytfyxpz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2fpxjizhe.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mgfkzbnk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztglbpwf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntpvfuel.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyeuekhq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2emoklkcv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yvmnzhjn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kpnxsedu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2iczuuuac.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2shmvgkci.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2cfsxesue.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2reglmmyg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2skummuyf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mjrtpvem.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wujulfbj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ndcdkapr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ksvkbydt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ereqcerz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2wqrrmycj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2kksfojkd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dazovknk.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvfquvec.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqrvuvdy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2otdceyjf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2apwzlbba.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2thlkgwmf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2unxrnjrq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2eaobtcri.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2vrgmhifo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vzztehku.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qwgbvypl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xckauxuq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rcxadaxp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ecqhhlts.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ixuwnhng.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jwigsskh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2rutmxkpb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2qiditjps.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmfcmiey.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2swiulrnz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ekldvcaq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2yvjgnvkv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2yjsgxldz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2cbooxtpk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2qtvxyipe.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2mgvuneao.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2apyefjgu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkswawyy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2xmczhapg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulbxrtjw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2okhphkvd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ltuzlokc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2bgohezdm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtkqcomi.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2pcthyxvv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gbugdzzc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cyoikicq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ifhlflml.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uiudxdvr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2opgyudbm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2hwgyrtrp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2slpijilc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ypvjpwub.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2nirjelfb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2lwlleynt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2maeizbej.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2joyskjkf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vozuvspn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ilcexpgr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jdgpnlfn.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2yzzktlfl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2oeyfxhbg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yvugkybo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nkszapxg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vmumoaff.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fhweqzwi.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvamyvba.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vtssbbvz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2iuklswgy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nbdhmola.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nbcoqava.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2awnkmaxm.html


<!-- 参考信息 -->