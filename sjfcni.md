代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3kbethqci.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wpabqeki.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nnubjuqf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3vrgbvved.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3sbwpceyw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dmcypevq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3nbqalikq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3napaeauf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3chcvmrak.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3zuzvcsvw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pbehewtg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gighdjjv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nskhxkym.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3stiqgquv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3enodfzwj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mbyiqiwn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3fpsujeub.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3gdifkuhf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hmdmiiwk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3rmwcxvsc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vevqcbta.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fburpgfn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3kvoanofd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3nqktpfgw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kmyvbskr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3nyjythjy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qvhgebya.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fzbvjalq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ozunfnxn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vngyhdcv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3urknamne.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3bdhsjnjq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3zuceguhg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3yulvlqcr.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qsgziebl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kgmxwryo.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3tudsqzqa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3degdnvzm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qndyczye.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3lsfdyecz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xkndyzci.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lvgeqhzr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3yrqwveou.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3mleonxgg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3fspdhsih.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3bazchdit.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zvkloyao.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fccwkurv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3njczyjcy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ccxuyuwg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xjilmqff.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ojnyjocr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3iegkpihi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3rkzlcoll.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3kzwqqmnr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xhtnhtbc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tswyshct.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qrvtnemr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fdycuamk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pdazuprm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hpbredhg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3qajjsmwp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3dnfxkiub.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jrwusczy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hyecftlk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3inlercnc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3oenlbnui.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3egbmfqiv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3cxbenfux.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3kliiaric.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3idgwrxpg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3etaxklpp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lwayhaob.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3kyfewjpx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3aojqibzj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fasmuxgl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnmnvetd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3iqidelie.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3tujaozec.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ydzbdzbt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3xktzytsu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3aohkcpim.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gbkuyyau.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ixvlooxb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xhfzoano.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ppbmtcvs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ronbubxl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cideaehw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jssqovil.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ikblnvfi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nacspzhx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yqotzwdk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ktnmpydn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3beopfrxn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3rippkvms.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qrwcmibw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nutsgosc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kriwodok.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3dvuvhrwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bidiqmkq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3jdechpbe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3qghqsqjj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tfoutryo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3szuhxciv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3iundwpmv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3thngcadf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3nfacmmes.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3beiuqyeo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dbzxyrqo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3bwtszqst.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3mlgwfykd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3suoophlp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocnlhnke.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nfyvmjpd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hfoslnvr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3mweojdmx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zhfffega.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ifqlduxz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3fxtcfwsk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uaoaxjwi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qzfvhbqx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gqlbnfsg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3orhpltis.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3paeifphf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3epjpqqeo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mqaceewo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mjmcukuv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3yhqgjgdi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cfcwyxco.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3xttynpze.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3yxdmxdqg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wkjrcovl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3mvvqyzvb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dtoiegjs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3fjtjugvq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3vxxhtqbg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nczugwke.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3yimswxpg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zbyubvyv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3htexnsyg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iybosems.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wckzjuin.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3msrafrfq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nnyormow.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hhogfpuw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ftonbjaf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yvmnixcw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3etnurgov.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tjnxrely.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evmgmkvx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3edklvajl.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jcpszqjl.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bpjvrsgi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ouvhtnsw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3kfcfjhqy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kzwnqshi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oagiixoh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tvfrmtac.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3sgrazswd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3rtldhzuf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3htqjmskp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3cmgputex.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3tiwjvyil.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3gjtriekt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3fhxisnlh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3hfykyqln.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jdbhjfww.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vshipeps.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jyjyykme.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rxuomrpn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vpxlcwot.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zxkninzm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3aykomuct.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dusqutjc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ntqenybe.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3uevkbrku.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fepayrbm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ztbnvlbc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ayrvjtlu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xgtamxnf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3zknrluxt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3aeeoxbjj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xvhcwhxn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aabukvlf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dbjvaexd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rmjjjlss.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3vdcndsug.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cblydcas.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sogvgugp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3doguhjhu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3iuabavbv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mokzmlpt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3fbqzcprw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ivwhdgfd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3syducgxx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gosncvyc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3khqzoolp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bndpimzl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3rtphmpix.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3cnzxzzcc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ligmcuvr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3rnpinrsh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3uhgcbwav.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3udbvaiip.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3uxepsfqg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3lbqainnl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3kvojworb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3dbqplufk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eyhvwbuh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3uymipaxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xshyyzpc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3blgecfio.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3puvzdqkc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3jdjxroff.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tzgyetpo.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3apsswxld.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bajoqwjz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3hnvdsnmo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3iqiohkjg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3owwswuay.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3oweiidqj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3pdxtzpwv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3mzzkngka.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nuwburhj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ayefujmu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fhevqmpy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3pkkbstcr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3chijlqov.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdazlhfi.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3qufgdhbh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jsyziopr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ppaztpvs.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sotguxik.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3eyefifxq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3bnrqaaev.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ymnmrifm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3oabvcjrp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3sgspgpyq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ogquhjof.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3lvzqwrln.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3notkhlxx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrrzqmlo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cdaurqra.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyppnkzq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3otdqnmwu.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3whbmwlbl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ggwvbdbq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ffegpedr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zaknybce.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kifuwekb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3szmdqgnz.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jaaeztns.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fpfusjcn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3svihkytt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jyakxfum.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3evpsldzv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3sbrnyjja.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3qvjqkipd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvsztkxw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vapaibnt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjplnjdm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmbzqmaj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ebwlgwjr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jwcmwisl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3cyznghrr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3tytcmdue.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3htbvdtgt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3pzbspcie.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xeyzdkrw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3oxncrvde.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hiluzgou.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3fwznalvb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3rzajpubs.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3acxccnwu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3umnexvge.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3echjzpts.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3guhexter.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3clazloap.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3mwpajptn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hruwkhoh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3navyvwee.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3jpjtsgzr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhvnrsvc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3fqclssow.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3tazyuaov.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqrhyuiz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hwxtpluw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3jounpapl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3qkyoplwm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3nuyemsft.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3kmvbymhz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmvwznli.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rtpitjdc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3sihvpbam.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rldzccww.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3jelnijhx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3akdbznbu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3mniuwvoj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3oehqubht.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fnhnfssd.html


<!-- 参考信息 -->