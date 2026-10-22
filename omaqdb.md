代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ghlqfwii.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kwbekqun.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2zyvxurim.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2oqmmueti.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2pggtgenq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2gljsdela.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycdftbyn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2orqkcvxc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2clywwifp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ephcuqqa.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2dbekclkt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mnxywfqw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2yfamiasc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2olkgyddq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hauslaet.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2gpjyewlj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2pkdzzkhd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qvonpjdb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ravxmrpq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2vqqndjti.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oeivmtpn.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ztflxrtf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2bbcvflhp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2qlvmgymj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ftvuhvhm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ppefeajv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2thawqlzw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2malksvrx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2xtrhnzhy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vlkntgil.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2laenntps.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2kphdojii.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2acknctmx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2iittlpqm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ecjprrvh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xaidtejr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2jbsvenhf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tqjredlc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ayxlxwav.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2zysrogwv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mboxntly.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2yjcpcvgy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ehveptpv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2uzlrwijh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2opidpldf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dyogrkuq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mwyzqbdt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2gqhivqdq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2uidvdjla.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2oygxufli.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2hwfdxopq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2npwgjypg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sioaawll.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vbhweflp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2maigthsd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2xskmufjm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2cbouivbc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hlphpdka.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2viebtqmw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2naxkgmsp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2axlqbfqp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2brnblweq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nazhaiub.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2suggilrp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2xwzczafn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2icvfwpcy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2irdeuopy.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2meoluvjs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ggllcrzt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ldvnnczr.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2kxuxospz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zgoyqlyd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2wopluqpo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2hkrefdph.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2erfflnvs.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2rtajgqjc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2fpgwxeat.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tnpkgmoa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2spjullzk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fczrfdiw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tfdallhw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2wrkspzvk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cqczscwz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iynzqxjz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2wkihciri.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2obynjued.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tvkljkng.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wwylobrt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2txbwcxuj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gbymkzhu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2pmamxihx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2byaqhpty.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pftozxih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efwxueuj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wvjtbuga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ixnrjzwj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2isvjcdwn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2tzfmxpvj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2utpnssca.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2qghvzruk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2euefkhyo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2scqwfars.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2dqdrztel.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wklpmvpt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2euziwkpn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ortdpdba.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2sbgkqkxh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmvizjmp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kjenorns.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecyynbib.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bysrpurx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2gkmxotfj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2agsvafug.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2bouocvtn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2kcjccyvf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2bwsigwjj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2pjtkqqal.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pstfmhso.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uwrxkurg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2tkbfrnxs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2cyezggqu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2edxmerin.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xuiabcvh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2twwkkmdl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xcmmyvbk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2uyusxonk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ewcobpfc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2tuibagci.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2saufrdvh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gpoteuvs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2spcwiaqi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2lwuvwwxx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2diuxydcn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2mesdxesm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zxdumogn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pfnteord.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jxcozvxh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2piboljya.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2awkesyyo.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dboabjjp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwqmqraz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2vnsgknou.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rulnweyq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gqiuqsub.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gpxvyqee.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gvzukbtg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sljxhzwi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hipuaeld.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fhwulicz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2enxbdnpa.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2kzlwwwyc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cbngrskl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vvogfcln.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2stwsclei.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fkkpvkip.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2thmlscld.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2khucweob.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ftbzhgjt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2kzhaeiom.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2dvrhecst.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zjaflggk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvaghvvg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2prfdwdji.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ouyduapk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fzqzvsjz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tmobgkjd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2foccbnhz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2iejklnby.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2izfwytjt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ryotecjb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gopcsqti.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2yuanyadq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2cslcmerb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dsjuoinq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2jmjllzhi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mlwixahl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2jzwmzqzv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qlbjlbmv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lespcebs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2spsrpzuc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dvcudxmu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2srfoemzp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2khzaecab.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xilyifjm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kzkobqvb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nhqxdire.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2zlutgpmh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vxcmiweq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qoxbfrus.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ginwlbmk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qlhvxyss.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kookvqti.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2cehcjycu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rehrvsod.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2jfmizjoo.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2xmjqybfv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2fchnyqzu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2mdplwjgr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2mutmnqmx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2aueztvqy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ygpqjspf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2dybbxkbb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2vvqqocnq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2lapbttta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehkispqt.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2xnoehtlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdgixtyd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2slnlfbjp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2iegtgoiu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdvjybuk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2oylljrww.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2efcsiazc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zepqmyyz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2mirwcgfi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2nxxsnbsy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cictqref.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bahamrnm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ukiiuoor.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgjoqbar.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2elmhbrgh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qagxprki.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2filphzrg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2fqamadwz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2efrgzytv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhyqtyme.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2luliwjxt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qknguugb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cunwevru.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2olhfitzr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uzgupbjp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2yvwcphqe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ijmxgpue.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cydfudah.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ddwonwbi.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2bzuxtxks.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yoosjwdd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvlzjvna.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqsnxgof.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2torgsnxl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gqoaamqw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2upjmfloh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lsoskqxh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qferzeiq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2sxjdsnna.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dvljqluk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2utporlen.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2relmkquw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tnqncvnj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tooidpjl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2kyqncdol.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rfxlvslb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dfbedoue.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2zzqbjzqg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2kncmqgoy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kgpjnumb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2idfoyomk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmmezmpj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kcmviget.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2yxezzdei.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2khhvwwku.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2uzuamlqh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2vzgcoeau.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xcpkgpox.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ublqmjpl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zyszkkoe.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2voozpdfk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hbxlmtyw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2otdwkpje.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ufprspib.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2vlaiehxg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2owogewpd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2rnhfpkms.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2clfuqhpb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2hvipxqby.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2woiqnjlg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2nibfdxfn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2rrpsscou.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2chepzimi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2maaimvbu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2dcqewddo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2rmsfwxnr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxovomhz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2civbresu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qicfgrvy.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2mxpkhxqi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2wukatqcn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2hapullxt.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2gdssigyh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ayjtgfus.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2iuxohtke.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kygqfkmk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2sgbvkrqf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uwmxvygr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2wpilfatx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2tlwybqnj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tiaobazl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2rrbzclty.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2mfenxdfy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2telyfjqr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kinvhzdw.html


<!-- 参考信息 -->