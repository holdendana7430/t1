代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qzjqibrs.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2uwrfdefc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2glxmlleb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mjndsgmw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2rrtowrhz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2jckbuimc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2npkpapzz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2uxfccagq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2soksnlnz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jxikasab.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uruqidig.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2prwazvmp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2zfzrisba.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dpwiacjd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dihsnhrd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2qrlanysd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2rikdhsbv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2azymwalz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pxmbhqae.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wlfyxewu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2yucxtitq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2clgyxxzp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2moebryay.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2avzaurlo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2lfjbtggq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hmbbxuln.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2kcrrvihl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pvzjzete.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gzwrnqpe.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gwaiecqm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ujnffekd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fqhbkvwe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2mmzrydfo.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kxgewxqr.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nlhfmeld.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ydcjhovv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bsjvczet.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qzghorwb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2esyativl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yyxfhgut.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uytjxvzu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ynjentge.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2faieejdk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2joqltrum.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2titybqey.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dwbguiym.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tefhsiih.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2xqenhzpa.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2bsrqadxu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mdnufkjp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2bmfzzqft.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2wcxgnqiy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ywhlcrvi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2flokffgm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gluxromx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2htjfdugn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2faoxrlep.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ndqqyxqg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2purdnlvm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fplrilbw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2xcutfflq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2qmknhhau.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vimvuqcx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2hgaewczp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qmvjqyfi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gjxrkyvi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2azjubazn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2jszzttyp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wwzorrjz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2fmvkvthw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2oyagfppk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2tmvcjzxb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2xcbzmais.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aceqhhzv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2rrvxwvst.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ggumszpv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ntzphkep.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2hbbkotve.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lrpchiuv.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2xyjsajnt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2qzgivqbb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2yfcjxkrm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jgjjzdzc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jxozgslm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qvsaxdyo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2lknaxwbu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2mlgnlfpk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2yusljred.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2hzrzfkau.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ieuvjbap.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rjcruevt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aylgmdjh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sszrlpqg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2fmprkyde.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vgkdcwdq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nyoarmzy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2njsfwhdd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2uuvtszju.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2vbekgnby.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2partstko.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pkfryxqi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hwfrrhco.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2krnqbtpj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2mpguccey.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2dyzvjmmb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cdmhzbyj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2swzjgtgj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mgqhinhn.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xcbjyvci.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tokznahk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ywcugowo.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2nzmkyczs.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ynpyzost.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xwkqpqfg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2aembhqcd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2mrrfpriz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2xurrzgct.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xgqfzefh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2futssggm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2idyvwesc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2bqiuqarx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2dalfcmpb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqzmhnwx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2mueojger.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2efofavww.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ypawzabv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pqjavlbr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kjmhgcnj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gncupcmi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2kbeqvanb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dpcaujfk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xgrrfcoa.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2tckhbkum.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2qlnqhoyo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nxqfpowc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tlehdxrr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oldpyzbb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2snizdrhq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2tevbrgxy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2asbtwths.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2afjetowy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yermextr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ohybbunc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwxmksfr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lgfaqknj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2vmarcemb.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ljkxftyc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2rkdrnypg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vpwxnggx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vxugekmc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2bwcxyyvu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ienhsbkf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qszbyuua.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2dvvbjmtq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2srdfvguj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2erhhrtuz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lhxvhwet.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnwzbtjt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pnxunbkg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2dqzmhahl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2jxqixqys.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2htjnkecj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2lxomysku.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ebnzytvi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kzfinohb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zoorhduh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fqihbjpy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2rqkimijv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2bijzkjzy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2tmuudmci.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yvmfaute.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2pgvtdook.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jfugscgz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2beioecwm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2brpgolte.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aztllddq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2wsnjeylf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2krllksly.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2iompiwro.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2txeunatm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2eghrwixj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2qnfymuvm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2exoswmey.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fukedxom.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzcoicnc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dppzvpnk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2lqtraqub.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vzxfhsfp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kxmqjjnr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ufxrvkll.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bkrcvbnp.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pdatnsji.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vokzzreg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rqecohwf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rvuiogws.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kihbwybp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qnuvtoxs.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zcunpfqx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ojotmuqg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2nagxidtt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2chgmopjz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ajyufgcm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zyycrfav.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2tarnwklu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2bpcuxvsm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2crlylcdo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2fddnvguf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2yycczjsv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mpkjrpyg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ekshqajd.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lpiaidwm.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2chyqdiae.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dsvracoz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2vagddxuu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2vrwstnvt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2lmmrvllq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2lwiayqcl.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fehvetup.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pdujomcy.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hsvssfaz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2odpxqmnh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jntzdypg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2yzspddjv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qbcszmay.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2nxrwbttk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2bmbzogdq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uoloqksn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eacpjwts.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mbdpzsjw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oovbbvwq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2rvvewvlx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fvrwzxqw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ngyqadzk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kctmcche.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2pxluiwsr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xijlipwv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lwswvqyr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2niknyocx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bkifjpkc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dywgeuth.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2trwrmoxt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ouepawuk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2fxwknhhd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2xiikkbfr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2idpuhpem.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2meonpejr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2cgyeluzn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2wmwmcjhy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2nhdouigt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xpygtoif.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2tljzfuvb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2copssvda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdvlvcrl.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2detfdkco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwkfvpdh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2dizttmjk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2lsrfyghx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2wpqadpkr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2akalgjkt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkgpwqqy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aiefsyif.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2nbttefii.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2bpzcasub.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dhkeeeks.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2qinmyalb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ycrcipzp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ippcfsri.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxqeccma.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2dxllytab.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhloggcg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2vbalqnrr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2lbxluuqn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lsuqueco.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2lnomvxlv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pwanrhrl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ikcwhylg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rsmjtduu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oggjoezo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2wtblatek.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2uynzfhef.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jndnryzx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hdcokozu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wjrdyiae.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gqwltyti.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tljmebmo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrseauze.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2snthqwdw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsdryfqy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gcdaqptx.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xngwzibm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2sqceehfv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2vtwhaezq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2fdtwfklw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2imnhkurb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gwgwhfax.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkmwhnyx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wvineupn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2pryhomhw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2jnmqvwyh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qylqwdyc.html


<!-- 参考信息 -->