代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xoubqjdf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2nhxbfdhe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nempbikx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2hwxftvhp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qlydfeip.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2acalukyh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2pggavzbq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gmbjlcmz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2vpqvhnir.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2injsbrzd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fzrjtcmz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vdrieuml.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2wwyzeknp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2yyzhztet.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2edvbndyt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2axlowelh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2enrmomtx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2cphjzveo.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2uevyvrzu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ushqbvis.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2egtumwuw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2xcjnrysb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cuojggyp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bpiccomi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2awqthbon.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uwpotkbp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lbvghoay.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2mbuwnkye.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2whjakieg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2oatpzlmw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2mptxwnna.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ocpldyfv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tshgrtxo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ehvkfcic.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gqzpokwj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2umdrbbxy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kahlecuj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2tuesnami.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ikomeltz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uxaeypux.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pddywaiz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yoxzjetd.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ayrbsmqa.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2tyegzwbz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2jkfkhwbf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2idlszehd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2uukwtgft.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2jibrpaff.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2uouproub.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzokvuey.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2swtrrshr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2amnoyszw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2dvkbmmbd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2qfofqxge.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vxdeofaa.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2zxguvvpv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2zwollesr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sdmyegig.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sjcpjcux.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cowhkmtu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zptlcubm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2yzixfjxp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cownmkoe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qnrluizl.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2eycuyqmn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cbqfdgud.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vdqndmmm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gvrrvltt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cdhsrfiy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2oidgfnoy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ljbipqnk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uczvvqrv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xtuzhhci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpldeuxz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2yonamogi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jofczucd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2imbvuoqq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2wiilklbt.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2arpbejma.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ypcircjp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ooiqcrrg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rlpjgqsd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2xpvwskwl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eflmnzta.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gqnmhfsz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2gqlqaldg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2yrjozlyv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2citohppl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2yuykuxmx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2uvutkbjj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xrjeuaun.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2eystkbzu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2igdlkbjc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2gddvyrne.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2qpdbtfmf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lmnygtlk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nalbclrl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rcnnmhrb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vjtemzng.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2kwazfsvp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2kkzugoia.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bqjtotye.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2svrfsypn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2bqzvopsv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pqgsavwu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2kswjkvij.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2atvqndml.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bugqmuop.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2zyguncuh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lmqhtldw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2yibpiwdh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rndhhlou.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ygakllju.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2gnujcnnt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pwxiabom.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2heksrjhq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rcyfrhds.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mvoulakl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ibzydxyl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nltmijjw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hykpeilb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2gmeqsuan.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vydftwjg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kixdwmhg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dpjobrde.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aoxlqtku.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wcdhgpqb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqbqliir.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rzqxfbup.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vhnrptii.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2vzcnljnv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mfqiaiwl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qwgdaxqv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wsifhbim.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2viaayxjj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wtpkgycy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2emtgrvug.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2wqwfwrwk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2unruplhl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2vtrorayw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2dxrrwept.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnhpwdaq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kijcxirh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ydsvcjiz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tfmczevn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2kmucldmn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2rlcqimxu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2lcpressb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2vdtonaod.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2csfuzxei.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ftlumdac.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bctmigqn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mmxrnbxm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2agigggrg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2zhwzyuhz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xmvhpoit.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2vspbezqa.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ztdtkhyt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2enymqnkj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2atrsfyal.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uyragtpj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2piotupgz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2iiwoenbf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tkelhqai.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rnmdgrys.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nswqtwxo.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2qagkzztv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ortiiyga.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ykbmpafw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gqokegoc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lxbevssl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ycrxcclo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2azarivew.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2igvwzrlq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2bralcnzy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2dundayso.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2pxrvvjnq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2hwpovjyr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2fnxqhttu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2rtphcwuh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2yignmqva.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2pwbeqrwk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2trrzmtez.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2xthswzdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hexjrofi.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ccwizhcb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ocoukven.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ijzlwdjx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2emyktsoc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhotwdvs.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdqwpnmy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2smlmigbo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2meunhuvv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2jzelyyyy.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ckdhgvjq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqmjujpe.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2zkbstzxp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2thovqcph.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ginunmux.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwqrkofo.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipwjtidc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxxnsczk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2lbhkaelj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tlzxteyi.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kwgbgiww.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2efcptrrh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ikuvcucd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tttvbotr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2avoezndh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rwxefxlf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2kjjzbgye.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lqijzsku.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2sbkvxpyv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ywbesthz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2crrvhwgm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cmuywwti.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vejadmjc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2epozcemm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kmmbbwlk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yfzffvut.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jfikjmqh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qbkrsbtr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2oeplyunl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2kyhverpo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2sfigqwju.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghvhpxxs.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkmmunko.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bovyfifk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tqbobsxr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2pknyqucx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ztaowbhs.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2lbmveskt.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2xdlfkahm.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2pkkfgwkf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2chemejzk.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pszsqfiy.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwoufvji.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ljunrydk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2xtacgpyc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ivrcqszc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2yizbqrhy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2wahpviyb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fskhvznz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vluruxjv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fwwribrf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nudxkecc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zrgyvvea.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2nzuofcrr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2lqjxqgeb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tmfvlxva.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2syqprifp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2eilralse.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2vpoywcny.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nvqgacch.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekovfxgz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2juxztzny.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ewzstxzv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2wcdlnncu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2aezeqmbq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hggutkbx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rkrplkiv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2cswdxwwz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2xvfupcvt.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdavbpyk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nggskcmo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2znfczsjk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2dvdfdmfa.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2zjfwsgvo.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2nyflydjp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2duaewkpy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hilvoqlo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2vrqezupp.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hgswlijw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2rvgadmwp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2afxyoppw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pfgypvnb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ujqursdd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2kpfoblnp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2dvcdwodq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wvnksmjk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebzikzcp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fyufcmbr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zokohswu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fdvsvntf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2yoyycavu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2pppbcpfm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2qxvohhws.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jziumqrg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysticimp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ggoiihrt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vztgixkf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcxwpooc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2iecuslsw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yxsdmdgk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ownwjekn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2tfsdhxay.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2jqotxffz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zwzzglud.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rrvwznqy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sgxivzup.html


<!-- 参考信息 -->