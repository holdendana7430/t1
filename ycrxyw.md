代发 wailian999

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3qqgfmrar.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dzdsvqej.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3kzawtkuh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bgzaaqip.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pelkgzvx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yauadbwb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3odpvwcnz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3swngdwxy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3opdpehpa.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3rrvcidyp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3rclrunto.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qmagidpw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nyvhhmpa.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3anjlhjuk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3acdfxnwk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3xmrvphtl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ojjszfpw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3pmrfsoad.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3twpqvfnu.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3sbswbbyk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3dfqjcxbe.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ebdxwkup.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jmbxwqru.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3djbdzvdx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3kkybpfih.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hpxlpphx.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ysxatsfl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3fegqhxjt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3bptkoppz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3uceezmkj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wycpvbux.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3smidfptt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ymjbkkwk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3jlumgdlk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vyjkwjox.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gizixjaf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3idmieubc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fckcnhpe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3hcafbshu.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ycwfnlbc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jaoyrwit.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hoatiflt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zoqkzyja.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bmoclugz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ecnwepvc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dtmrrdgk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3aguwevtv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qszujonw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3copycppy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ryytydoy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ebizoifw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ixuesoac.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3auwtycmr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mlstfchz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3awbiwvkm.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ohmtofna.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3pwptaqjx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3srnlptvu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3tjelrnql.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3aiddrrgm.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3nluenofw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3iyshrlxb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3sunwbjvl.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3etvxkgpg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3tegkxoow.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vqjnvgpd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3btijyttt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3puooqjbg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxejyryl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3btyapxhs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wksvjjgl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qgkszyaj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3aymlmvvv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3qczomqyh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jekbvigw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3bhhufhmj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3sycblmkl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xycthavn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ffwsquxn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3cgyxmpee.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fxpwkzun.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3oqocspwt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aiabhppt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3mkkrpdru.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pocgkdqc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fyjnwmcg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3wbemcsxo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hblgasiq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3wdmwrvah.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3wlcsxiui.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3reyhtrga.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3roskeggg.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3foesxcxe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3yephldzh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3gadthjpw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zrulbtnd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ilcncwne.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3zkxjgibu.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3tovqustn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3wukarmwr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ujaubvif.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kdwiveqt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xtywsvhu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qfdoslem.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3vppkmzhk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3oghpnxbm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3yhuesqcf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3klpualmj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3thvlihvz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vneucuvr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3jcpabsgi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3avzjsfse.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qlmrygve.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3akcirira.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jjgvdmkw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3szjrmvzl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3zrmlbfkg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dgrqtrbn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3zbcryopd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pwetryzu.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3erlysisk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cmyssvjv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3flbvpiek.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yuzhxupd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3lledigte.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3lwmgdgwf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3apqbidjx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3djwjoqte.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3njavtukb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oapagjhf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ozphzccu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtmhvsnm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rdidvusn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3xksjiixr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3abelywlc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ivbadnmx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3rrqudlpw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mvcdbpwk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xueuzjoh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hdyhexru.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fqjzvkco.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3olmijcjj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xkavasjd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xpzrbmpd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3uedeizjn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vzgkbqhh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yttunknk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3daiavucv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rxubdcku.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pjlvuarr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ptheclso.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mnbcqtyu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3btzhzvvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbwvoflh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3xzdlhutp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xpgdxnhu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3omffvsjq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gabpaymg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lzgezedl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3gvhszjtr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wvbmaajg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3aznzpuno.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3gutvlghp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3icjzeupv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fjzsdpsf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3antbjeeq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3mijesrqd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3cplsrero.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybmlldrk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqpojcye.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fhyneikw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3tywxsiof.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3meafbqkt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3wavftihq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3igodvbuy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wtaaydlm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3akpgqptm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xiglpssb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kcoeqgmj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3tmmpjalk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3hfzfadsw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3psjjupms.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ejvqccip.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3lfguxrfk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qfvrwuwt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ksfflhzh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3bzvrukln.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jzacraaw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3thwtxkvx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hhfifear.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3gxmsbsqc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zclkjiov.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3rshboamy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3qshcaelu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zhrhibdb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kxnslmga.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qpdpplsm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kcmmvfel.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3qyqsxbnw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ewqjwgej.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3akibdeom.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdtuobph.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3auopkheb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rqvpdguq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bblekmbt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xuntxeda.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nwaugfcn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3thqkevho.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rnjdnzww.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3habseuby.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3gygncili.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3yugngitp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ogoftsze.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bvydmxin.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pdtizucp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3dhnnldpt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3uwbcnuov.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3cmxcldbm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xlcasymw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3mcalsfit.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3pxnbrqwt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3audzkwoy.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jvnljtjq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3abasdqkz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cdvwbkfg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ungbbwde.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xdjdscae.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3lelovctq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3brtngkof.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vwzvbimk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3buvycmhk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3iomthssk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nbrdzdqp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xivbmztp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3vvmgnsaw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bqsslvji.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3iccwslxf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3hkxobmpq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ejibsibf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3edyhnbdh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dszwmrld.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fzuqkjws.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3pqtnzwwd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uabiyqwg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rcknmuew.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3guvsqjnj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3mczvutpu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mjfpnigs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hwjdzyxj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gaeuodyq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qmgqtqef.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vjqqcftr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3toycsxsm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cohoobwm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3sjjpduuf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3hddsabrx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3vwuqeulp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3eegmzeec.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3xafshrgr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lbnmlxke.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ydcdkfet.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3rbaarafs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3cwkhpgas.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3kiftpwtu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sawprdns.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3gkvtitpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgvwpoiv.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3vffksdmg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3bynkbtaj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3qgiunzuc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wvjxgcit.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3niotxdsl.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eilkdsjj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3saocrcym.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mfiboqea.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tjmawwyw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xbfyykhr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3wkjuqdld.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3hjvnlvsm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ltyubupv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3onbnyqwi.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wfcfmblp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3nvrnqbvi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ctwfkilf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vgsbxfpd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3lbiuswjl.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3egqxbcdw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3iflnzhfx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fnvpttup.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3jozqbqvs.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3xklkppzq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3pbgzogrj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lusibqez.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3obdjqipc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3pxeolutp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wvqclntz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yljssffx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffqevelt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3clschexp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xnbkrkbm.html


<!-- 参考信息 -->