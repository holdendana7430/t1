代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3cfegeaop.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3exoygjms.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bvfletap.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3wzrwesmv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3htkhvslv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hoeqaaiw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3hvsvntsu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3bylchscm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3sjjrhjwb.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3lsqkhdxl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ckoqdkce.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pwfdczga.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3tbthypyp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3zvqgztwi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3hlbtdmjd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3srbdasnh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ctswldkn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ucnkxkal.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hilancsx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3rihrnrba.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3yelqmucn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3sgonrrmr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zrmzcdom.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rvpmmebd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hbyeuvmr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hyxnxmtk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vokhiscl.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3dxtoonnv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3mnqgtivv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3bswgmvif.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uudqscqm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3drvgsqvl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3eaheriec.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3lwxrxdhj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3czauhwpi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3xcqfnwmc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3dpbxavtz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3kvxixpxl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3akvrmvvi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jqtqzshz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3furyvdbo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bgkmjozp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sdatiykg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pmzmnnfx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3xufebxlv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lssopwpp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3cydnpsoi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jodklupc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ggyibfdu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mzcgxdub.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3dymzdgba.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3sqefksni.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3isepsxbj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3yggbqfer.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3wblxqnae.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3akknaitw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3uolrxxmj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ikckerng.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3dcnhjdrk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3weaqtxdu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofrpfjpz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3mepnaxtd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhjopfkt.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ukzcxfhz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3itlfrzin.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tbybkvoa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wmetuwck.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pqntindd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lizznzzr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3uvwznkci.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rotyuktp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3raeuyspn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3xttogmor.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uekcpyxy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ktmzthsy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pruckvoo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xkugghuk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rxtvijwz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3oshvzyhe.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xuqyuxak.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hkmwxmze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kicipqid.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3heytewfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ytgkhwww.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3akhxfgph.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3qsilucnk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3etuqfizh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3vosegtte.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3knguwihs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3btenaczp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ssbtpmkn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mhmnwshp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fhdghmxj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3epiqyxao.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3iiwwhqxx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3evkyycoq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zoodimop.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbttxnwg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hohroysm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3subrbpoc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3lsufbwqx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3pntjxdqj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3hhrizpcb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3rzefbpen.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ypfqrkrt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ijbwicln.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pnywsesq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kdzofxkw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3golkslix.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3eaipaxez.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ibfaxmft.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3gzvceqij.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3quppkylj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ndshokym.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gsrhwaot.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ctfsxukw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3qmusalaw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ljoukkan.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3mpgxbptm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jjjalqhx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3isatckqr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3kjeqtsui.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ywherplk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3donvjwbb.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3itptkamc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cmawrktu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3rasibmzs.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bywybnwf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pebhapwl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xeelidln.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3olwklfmp.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lsacbzfg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fcmwzjup.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cbvxrtkp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jprobdhw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3udtguxwy.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dkpsqxmj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sgwkvonj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3vsuanqot.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gekdrrvc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3qivxxcws.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3sljftezn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jzbskpiq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3orwsmuje.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3mmzcmukq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qvkmsbzu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3tydoktmo.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3pavdvuod.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3jytcodit.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3cweudjvx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yzoyafyr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cqhquyzm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3oysbqszv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3batzahko.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3eynkqraa.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3avhedsyz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ffurspzu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kalgrmpg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wqpgkmup.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3aaiuoujz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gykdntut.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bmxkcfck.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zeobnshi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iqevmkce.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3amjijsop.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3qwhebbve.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kfkfbwvg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wzbnnsiv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nfkbypwg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wpcwgwin.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3meyvaepi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3udtfyura.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wxsrkfiu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ihgrjirm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cwoljzwe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yqtgemoq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ehnhhpws.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqgyotsa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vlynqqge.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3auoxcrbw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3vonuxryv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vwjvxvoc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3vqbqlyeo.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xfmxosij.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3gpwxgikc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3aoucaorc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3otmmeelm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qmbgaylz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ihnncuvd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3dcoztfoy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ctwlhhio.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3jrsqkgjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pegnqjcd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3vssbqmih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uetisftp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3axiusdyr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3joxjxxfd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3uvfbuptr.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ovpfgrlo.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3gzgqcsvb.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3bababtyg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3sutkqvxy.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ivptvniz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fwyybbrm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hnmtmhde.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3oeiatazr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhwihzga.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fdflstlf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3kjqccnlu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3aprmsgsl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3wgairrqg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ixummwwc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nicswpcn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ojpnmrwk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3avoniumy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jumroiri.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dmfenxbe.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3yaeutndp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3hvvjgfex.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3tlupzqec.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3uzhvshlm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ntjqehku.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3usluhflo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ihvvrigs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbpxxavo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkxdreal.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aprgzgdb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhphgwyc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vqnqyulb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3sbrzhpoo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3auniiwfn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3aacqqyoe.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3drnjjcbh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rovsuldp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bykfohtm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vnictzba.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cektyqtl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3emngrrnh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ujkechvb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kuxumfrp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3pcddwtpm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3jbnqruho.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qaoxhdws.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3clwktwhb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwntuajf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rrwmujjc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3epqwotce.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rqrvhrti.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3smnhzodm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3frglrxiz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3axlcgxah.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kenjyufg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xkexhlal.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vqgpxyvp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xxmefopq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ihxoobfn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3hiyxzptr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3stjcqsvr.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3wqqkrvwu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3wjcmoidv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3enqwhsnc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3gmvfadte.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3wyxlzjau.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjxjvafg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3mliixamo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3bcpcnmcr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cksjihvg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3nybaxfgu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3hdlqvhzr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ovkomkcm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qjhvkzog.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3yymubqgw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3vcfrmjpd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3aicqfdcp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3wwoptsul.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tyrhdevp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3dxhfviwl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3xviqtslt.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jewthnyc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3vtvvgtot.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gpizntfz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3nuvqgwjw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3qiqkrlxt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3viqiagkf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3kcbnlmgc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3osdqknns.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ocnxsygp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3smiojgey.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hgiyytda.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpnxfnwl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kcaofbka.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vcdynyqz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3dykistks.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3otaobyof.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3efouuxex.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dhkshwll.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3itocipse.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3guqtarvg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3agyodnjn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3edjnscqy.html


<!-- 参考信息 -->