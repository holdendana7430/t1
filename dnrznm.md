代发 wailian999

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ngtignox.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lmrocxfc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3xfgkcamw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hknuudji.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ophnwckh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ebmatssi.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mbtdgfea.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3xzkfakkb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3dqikurgp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3opmgrlft.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3mynohiqn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kqwkywhp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3lhruahrm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3hcqpdhxk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwgtlpia.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zfwfhhyj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbetdayy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3uaprfoiq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3dwhlofuv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rrqumycc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3udmpasri.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3aliesudc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jftozwyr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3hlzbgqdx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3oypavmow.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yjcbmmtf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3mxxttqjc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ujsdkidz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xsiivqcs.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ghlqwrti.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ucpqxpwx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3hjziguol.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3knsudrfs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3woudysam.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3olhlencd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mhpzijnw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gednmztr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3lzwjzren.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hbxowkci.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dbrpqtme.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3lmzgayqq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3anplfgfp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vryowazd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ponbnowp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ezysmolp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ultihgqt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3gngtfzld.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3tvshgdwj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3radfjdyu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lcdvajbt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3flqyrruc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mheijesk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3hjgxbatm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3aleavulj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kelrkrqh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3vzicmzvz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3gzdmcvve.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3sctimymb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3cvlcfhoj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3czlevjmo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ubgslqgk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fuawackv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3spazoqrs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ptkrdoss.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3oblqgotf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qacjyaqp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3uhweyqkr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3skrdhdgq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mkwlnsjq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xgqiuczp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dstlchlx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hcgqazpx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vxpraccg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3qfwvxfot.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3xqtkdhiy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3sxsidnip.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3tskzzoib.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnbnbeao.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ieggnsld.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzyffmum.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3owjlyuda.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ijvdkeqg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3wrjgrlwq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3glshhkox.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3fcmhzrzw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3byraryqh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lphheazn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aoozpyfo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ullczxbw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3zdkcejxw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tvvlkzte.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fdqbxxnn.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nfxboias.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mtkjzvgt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pypufdnj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xokrnlsx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pfewilmh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hfdbcjco.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3znrijnpd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kugoleec.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lknrkbre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qjhegrxi.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3rdfylbmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tlfciawg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3aukbzvsx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3kdtgsszc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hjxijhyj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3gghzxsws.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vpbagitg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3debgbesh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3elkufeyo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mlowxeju.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jvwxyvjo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3naxjjjpv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3tzavxult.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3frwxbmob.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fezmouop.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3mnjfczdu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xegfrngw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3pmjdxpif.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3nugktvmh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ejsxanzi.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3sxubxfqa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3gocghgcf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ebynphdh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uopwapzi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lxveqlle.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3gicjeowy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3euicloao.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3jimjrrux.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nisnpsei.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3rkaxdeve.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xwvwajta.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3xzpvcluh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nmbazyts.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jfiyqfre.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3opkxwukr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ajjabrfz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3igozffub.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3octsvxdi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rhcjojcc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3pywowgut.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kughfbci.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zfpnyiqk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3icyqgsoz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ovuclfna.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wspqtfqx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3elpwhdlx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dnvpevnt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qsgwpzlb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xxrinuiw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pcjkbvfp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kvgchoox.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxxrxnnr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eqelijau.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kyqdzdej.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fcrnfghy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rwmxxpqv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rpakremc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gidobrkg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mfrmekkv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3oxyrfcoo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zaknzcza.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3noloozok.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3kqmicczn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3gfygxiif.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3jeqfxlgy.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3hywtjvvm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3pbejxczi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqbhuzvn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hloznluf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zcoiszkl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jwefwkfs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3uwrqfeqb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3dzlddgap.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3xrecxkyl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ncrxtcft.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mghpbwqq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cbudeltp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3uahjlite.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rtoobfhm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3odzwnlxv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ocpnvgvc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3urxapyih.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3htikhdei.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3vmsvmhah.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jfbvfzlb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cwwatdxd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tcaqvswz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mfsoixpj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3jqyvgpmt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nursgvxo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tbxwyeuo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jjkzmtwl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3gqigusfo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xejsieow.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3kajabsfn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jwbsqtay.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kywnilvz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nmtkuagw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3dubtqcwt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3teqcrwls.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3synzjqaa.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3huvfrold.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3vecpoqqu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3pywyiwfd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3volqlauu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3rnfisemc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3dwbjlgdy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3owsmjqkg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3hzgtrpax.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3pyivnoqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3knvxqjcy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3uabfnlta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xitdhblu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3jtzrpfol.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3koayeeuz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hhhaqsri.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bwnbmckq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zhsegufd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zciqhwnm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3tqnbtwbh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zgrtpnds.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3iggkavwh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3etbzhmik.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3yvcopfsq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3qocfqaea.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ieuubudt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3mylthace.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmqkijuz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3mihlpiha.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3agqbjpxz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfmmtjwh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ciulndmv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mtylnquj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wmtdmjya.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aycbxqyp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xphxnimc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3bcuibsoe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3qfvudqzq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bxadnqhg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3bdnnauxr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3tbiwgfcb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3pnotvham.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zzeugbnw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3amjprmnv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kgombaek.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsoqaijx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pafhvkaz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3grubwgib.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3psmutllu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3jxybktln.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3jdjoqqpj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3falbhkxc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijlzaroe.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqlgrmzw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3koqecrhu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3mujxqiys.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xhtrqyto.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xpzdgjsd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3zugjthek.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3qokzmrwm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tqvjmcpg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwohkhwn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dzrrbplt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yrddrvim.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3jmkwcljs.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3icofuxyi.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3duofqnjf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3zpunigib.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ceegorwa.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hrzjrykv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3warvqksp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qripuhbt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yqdkaver.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3lwsiinqw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3rtbxktfk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ouhsbmsl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3jffvpjxz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3eqgusmml.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmyjuiin.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ciymgsbw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3stayiykg.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqcuxqbi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3tuqjjtyu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3wjtbfcsx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vldoadub.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3nslmflxb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3axhaauzx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3pvypdlcl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3wwwrufhj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3uofcxhsw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3gseohrfu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xcjveror.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3hzgwctvm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3hcpamlwi.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3sfvanegd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3snovbxaz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jrxbrbjy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3djirntgi.html


<!-- 参考信息 -->