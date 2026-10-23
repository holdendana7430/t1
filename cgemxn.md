代发 wailian999

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3nhasweid.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zbaxdrtl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3izmgwqae.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kkhfixam.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bagaxmot.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3aojdllor.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vemsvcny.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gsulsyfi.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uzipxdgo.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nqbsnbss.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3axalyieg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uxgbxusl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3osayisph.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jlqdwqhx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3jtknjtut.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3yjxjciiy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3yrbigjoz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3uagujnnd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3pgubfnry.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3anzvlzng.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3pptsfljf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3drjorpne.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3epynzuny.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pwuumdab.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3evcysosd.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wqfxocyy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vhcrcurd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3fnqjlkza.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3brkmugmh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3znwxzcgp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wdfiftbb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gtrlvrzr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bpdavxft.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3akeblnkx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hpktfvdh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yvqdqpmm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3klzpttyp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jtdwqaxg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3rpvdtugq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yfniccil.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yxggdaml.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3eixsgmdq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ccznkgbw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tncfitow.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3umyonqzz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3jcmpldbk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3nlhakfse.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vmppcrzu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ddnmoplo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eqvwyefs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kxfzewib.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nyarhtot.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3pmcxhpjt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3mrdfayna.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3wmaonpau.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iyiodcvp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3tvkdslfe.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3aognzokl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pafturek.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3wldkqfei.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3odwgbvgj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3fchpmcsl.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3mkbeoahl.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ghthildo.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3qlwwobtv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3milxlytw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwmyrxsy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3huuijbjt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufqdtuil.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3xdhdnzgn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3zhoxzzoe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3copngfmt.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3fthdjsdk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3duiaoxfy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xsfrpjnh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jssnicfv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hecaslvo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3iehplaye.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3xuismrki.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3fzhgkzkp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ehcivdvz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3frqkuxah.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zyrmpfri.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3vtyguhbr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yagtkcdh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bngypkjt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3mjwrnfed.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xeiieupi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ztsxlrkj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3kaettibg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qjxaeroc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3njqxyjsc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3yhplilnq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dofpsunk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qizyugdi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dtozxdhf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3rtsxtyku.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3snmiklph.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3hapqujuw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3zxkyvyme.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3grwqgocb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3besoeytp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uqjcbrgk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ernohskz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3pnrxwxjz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ljprxdqf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3owttoolq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ixroapns.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ifpypubd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3clxsoqdw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3bgaxtxmu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pxkhpkvc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tmmdiver.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3povtmuco.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iljgotop.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3udploxuw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xiqhqnxt.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3gingxqhj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3nupkcgko.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uhxabojm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3orslllmx.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xozwdlrj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3zetftyih.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uohqwxfe.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3hcpiezow.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3kuztswsp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3qlvahzvk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3abguhnyu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3jthcsann.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3wrtetwwd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ucuxiqfu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zwjrgovk.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3uihhswdl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3pliedqyp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckuzfwlf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3qkrlxphz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3wlpgxehe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nlvpgwae.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vvzmagtc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3idatnloy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yocmtccq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ofpxeddo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ooprmemj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gcmzjrbi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ygqmobde.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ocwbuaow.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3aktquevp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3irqcqpvb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wkfkdpfp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3aydoxrjx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3jcqsuiwq.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tsxdxfza.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nkaqjxia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ipcghcuv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3vclqnsho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbysgixr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wemlsowe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ckpocdyn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dzjhmdyd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3bshzlidd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3irrxsdgf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xynxfqpj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3szmcocij.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lpjvtaia.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rzkrowrp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ngbcovxd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3rlrlkncu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3zgudsskv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyfipojv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gljknwfp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3twqtaizt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3psgnvqnu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3uvdhwvis.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3invstrut.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3lfupoeas.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3vzploeqb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vxnoxclp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wjhcaida.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uvtyseij.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3unvwzzxr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3nmbrzbwv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ugpnzowj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xsrowwqa.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3xxepakxq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hgmhezks.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3amlseypy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vdrndxof.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yofhjhyr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3kscpwtlq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3efuazrzq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3vvjqrect.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3darfdpkm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3voxyzmxk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3vgleuqbo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kknvzspo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lyqdqqec.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jmzafdkw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kfavhqmr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3vxqsobgu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nycmzdkc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ocwvvxff.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3gmwtugtd.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3esicigiy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kdbnwrcb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3evcuzasq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3btudoidf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fmwrngse.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ovlzzvgl.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ruotleaf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hzhnmski.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3jefxxkjw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gdxlarhm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3aeuxhjha.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3eoryjxfk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ldkyuweb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3vmtaicgy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3jwbmleze.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3aauyluwf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ovuzlrgw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3xznstkyz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3vfxgcvsk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3awimyejc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mvmpvjwu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3yakidncq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3gfxjuldw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3xejnvcow.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3nxzmvnct.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vttqxxfj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3cculqrnu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zjrywpsh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tjwbgcqc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xayefifq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gooqotmk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3amgvxsct.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ljsqojpx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3suzpkqyp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3olaihgbd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3blvjtnuy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nfaoxtjd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kfpsgyfb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fjofywrz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ajfbydbv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3dkrutmeq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3frznzwxa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dazhvygb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eyflgfyb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3rdcfvfrb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ysajndvt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3safngnen.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aeehhaze.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqiivuot.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3shxwohet.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3toesormr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hblonuna.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3vkjemtbv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3eenamqmv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3beizgaik.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3piajiqof.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3glpzryxa.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sdpqmcbp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vatzykuq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3nczmxmxo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3myszsqef.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3bxqvxepy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kybscojr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3aniktawr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpytxiba.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ugxfvzaj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3dcnpoeuw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wjglofmm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ryxnndjn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3verkirzw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3aholgxyz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3cvonmfgs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qsumsypl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwuzaezg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zedkxccy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3lyrnljix.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iynhjult.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3arfqjvos.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fztrczxg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wlxnhxbt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3rfyhpnvo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3oybcqsss.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dtjufuvo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ftsnyjgb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rcuywgau.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lhkeimyc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3leiwhvsn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bhlclxsg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3mfspbzmz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3erlrajod.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gkrxqwac.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3shcofaft.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3smpviial.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wcigdyqi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dglaeimi.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmtepsdr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rwidgspn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cefoaftj.html


<!-- 参考信息 -->