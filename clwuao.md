代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2padtjrnl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2hrwbhicb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pfhjqbsn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2qimvpscy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fchmzrdf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2leyeryyp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2wjyszguj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ioxdwida.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bmfiuhpz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2auykovqw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2grpweste.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zabnmvzr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yawiwvtw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2igczyoum.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2hzcvngub.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fckqdpek.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qaujezvy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qhuxkthk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2scgmjdxx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ylhtxkvb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2frnllgrm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2usrhayaj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2aygbbpuy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2fbmddfwj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2bzlhtqwg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2prafqtdz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2bhdjowjj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2vnmtbzwl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2bfkowmuy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nutkvcye.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2luxjuznm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bmyrjwmx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2shsixrup.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2sbjvexrl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2kcexcfcn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2boeagqij.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2espolpsj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2wrvluovz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2njzendct.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ukbfzzyx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jkmzotxy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tovkimos.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jcbpuava.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2liacavgu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2nqprpguq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ykxowhwb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2nvklcyfp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kzuzansc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tadirscr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2prbranhq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jfrynefm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2hdurvfog.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2mnkkuvec.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2iftxlfrp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2zzbdnlyv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2cnbaeawe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2rafonfwm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bagsqfac.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnzlqevn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wedwhylq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2eqhvlewt.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2jykworva.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkzkeyxz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2znilcvtf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2lyeuesna.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qpevxhhc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lzvpmlbx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2idwliiol.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wbcjmzwk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2rnprmlzo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gpvnqsxt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pkmbzqba.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2sbdnvzkk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2itxxgdxw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zralodpq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yecaygnd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2muejzupg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hexfhabq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2adhkpgza.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2luyxztwb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lucljamb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdqtfoiu.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2eyqcfgvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxpsvpom.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ihedipwr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2gwbtjuzd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2thvnnxwp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ynrwfnai.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ugkqbffw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2iacbfqfr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2pdqgimwj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zburkvmh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2psevhvui.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2klmolwoi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2rygprfbn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2rlepskkb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rmxsasta.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aettkjev.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2whpzwjpg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2tksmbaje.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2zwfzacvo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2kogwuubt.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2wwxxflew.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ztslhsta.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mbigthqz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jqcofizv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ovamouoo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yrhkdubf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2jacmtnhd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bvnhbxck.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2knznobxt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2hvokuehj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tiufyszu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2anggjbko.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qqxyiezt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2stjknegm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2wfbeanny.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cpphulwd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2zdjmoxmb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2jeakejfc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zjrtmeig.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kkbjwrza.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2myljcgno.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ifjpfvou.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2noahsbwq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bivubhsp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2gcmxundr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bbyxqcut.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2adnlzqse.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2huogloag.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zcjikrsy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fctriqsv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2geybabtm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jieiwnoc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jxbmlofw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bqusjvdf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bcacngyc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hvhqaroy.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2pbfxszxm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cfshlxvu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yssosshk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2neoifwkb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vlfqagtz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2dgmwtjdc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2fkeohmkl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2lbwkvmif.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2iheyenap.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ujtavxvv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2nwnqrqln.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkmcmrld.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kujwkbfb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jylnxmtr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2nxjzhwzq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2afubgnhu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2agxpiexo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2asxlizhr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wspdxtbs.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pjekdxqz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pehfyrzg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fvcfibgn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lafbpdme.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wstboano.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2lybvecns.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sahhwrnr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2pntfikoy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2diqtgqkf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vcaadofs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hvwpnjut.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvjuqhfj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2deocdwvm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ojtuukxc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thdbchbk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zthvwyae.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rxpvzdjy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ytvlmhpr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojzyfxru.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2awyylzsv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kyzgtsdt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ftbtmofq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yokwacir.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ihtnjrwd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lxuegwce.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2gbzvhyiu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2hrlhhddd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xoblpeui.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ufbcohip.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2jiidsxnv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jwvfuldi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2bswjjmqx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2amnmgyhc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2sipjrsou.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2blxvyiiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjbsvtod.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ttpjpzdx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojfudhlo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2lvivepaa.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ouwkvmrb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmvbdcnn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2amiqbxds.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptqehuxx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wojlufff.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2zypvdrlg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2jwxvorzr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlzrkoly.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cvqfswww.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2quslbuig.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2rfcgnfjq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wdafsdqj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmnycild.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbaxmlml.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ridtfcvc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mwlqiavh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2citrpylv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2yttmabwh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ahndxtzi.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nuoznkxj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2skuovxpr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2layfwpzw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2pzuwctpn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2dpfdmzmi.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xdjzgjvf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2znvnkozp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2uzildaqu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rowtcwgr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ndxlnxve.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tkowxsqz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zfauxvoz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nijnhntl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vjikubjb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qzzzjekd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pcizglhp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2jaaeoquj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qmknawbf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkanoshd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xgjwhtnr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cznhfjxv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2emhagkmi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ltefkssa.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xuaopbag.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ziiomfxf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2fjgveutk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2iyjavohm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2drpekmtp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ihtjzdse.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pwrkyqzu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oclaldze.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2wtznttmd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2zhupryer.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2rxcwldub.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2lgxgjxcy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2gghvlnqc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2doromnfr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2muxkrsmu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dqsoqead.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2esrhhdrr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2llvjucky.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2kksxrjum.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2sojicirp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2uheiodnx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vilmkrjt.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wbosntut.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2weerhiha.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbjbthde.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcpgtexf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2mmfdlhbs.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2fchvzyry.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2vtfzevwl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2dfzihqal.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2eqpfniro.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ogbgbvyo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2iopvxdnj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2wnookgix.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ylfobdkf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2uiwcxgjo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2lclkpixf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2dbnjwtfg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ekzrebvz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2idvbtmlf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rxrgilhk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2adaslyfh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2stevqfhh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2jgxpjlem.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2mmeeofxp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vlfyqhvs.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ergdivfv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2xjxwyqjl.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2axqffbse.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ejwpzaym.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jybxqeie.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zohjgqdv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ohkcltom.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2odrglfdo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2aezyuxox.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlkndjoh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kqjvxlkk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gpyrnzzw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2prynflgg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmqhwyhp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2srxqmchs.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2obkcyogl.html


<!-- 参考信息 -->