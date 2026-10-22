代发 wailian999

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2audndjul.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2gqdvaytu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tquzrpyq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yhmccaih.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2hhtvbbje.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lztloqtv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vproxsfh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2uyrctzua.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2sfldowxs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2khfpjtqv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2elhozomk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2flhrosiq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xxzemwvq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2mvfxndai.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2fbqbgpby.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2paxrgxdb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2pncwlacy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pwbfyjkj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vxoowlfs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yfqwlmhe.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cpftqxzn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gzccmslw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2olutbdgs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uvspmxnc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rmbyvohl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2xmbyqhrq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2beknuljs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vwdgeywv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2phnfyfgi.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zoarldrr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2jhcaelnc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pddcgucv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2qdpuyyjl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2yoyoyzvd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2mdjwtfjf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2xsbxlrfk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2tkyrwkyx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lilqbfvn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qbuubkqj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2yxywaksk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2swonxdje.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2akvgrkmb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2seglspva.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2eiihfcnc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vnkoamwi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2qdsthyue.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ibuknwjc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2iocrhwqc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wizdvowp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2eqalncls.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kpfxcuov.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vmhyrtlq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2gwmsqvqz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2imsruxcv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hvtnvjbt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wqozknyu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lsgmzupy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ntowityg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fpigibpq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hkkmyigw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2wozcdcym.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2njasoliw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2prfxeioe.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2aqvyenli.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hxzyenjt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fhaopbed.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2zirgmuvt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vhimrhre.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cglbdavg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2dhrgkzel.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2txavriat.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zqstvxbb.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2wftkryjy.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wnefznxy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lzcuvzjv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2hnrhavwi.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2dtyjspqk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zlejicqg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2nyslpegg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2etcnaqfk.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2cgislbyz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfrwozxy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hodwotjg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vjquieom.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jfqedczb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ueizufub.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2zxgbpoug.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dcjleovq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2sqlqiffk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2gcfvzocp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2kumsbzcp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2gyfjyfzn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xvsxqgug.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2igyomsrs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2osgqnyzy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2jmtohohx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dbbbunmj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2sbjtchks.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2avwyvwnp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2xptulqqv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2imlirita.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2oqebszpo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2wxfcnmfy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ywsvvvbp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2luyzdnua.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qfsnurvf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ogqxsugt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cajxywke.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2jhvzykme.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2riusnqdy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xgrgtnne.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nzlslxoy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2pepjochi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wqcmjukt.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2tzymukkw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2uftljnmo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2yfdvmopc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2mvezhxrc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cznmmutl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mzvysanz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2weiwtjyz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2aakzilag.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2sdjrtfbv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2kiamswmt.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2szrfqjvn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2yrtasgpd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ebrlcphv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yjtyeasx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jwywqnsy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2aphupscy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lfvveblq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2cjfugbty.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2jljzeuin.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ieulelzr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2quofugis.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wxieotvv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zqfxgmcy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ykbmiikk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2limgcbxx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iqbxrgyx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2nphwxmee.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2imfxzwfv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2uxcxqvym.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2kinxoemt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2vpelbejh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlqwxvuj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2pqqnvgkg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uluxobqk.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynzbxtnp.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2xenbdlbm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqubbbyt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2atqgqcpk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2jcjgwwkq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bdlnvynm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fgfcfqxj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2biljtcei.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ibvwutex.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2laiomagl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uhxnzcqv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ntflqbxm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2zsbaknuu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lwrcszfd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wosvqopq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vqunbqld.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mmrvhygx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dbztifqc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ibvmauzp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qutyhysa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kprfzmfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2angrvloa.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2okfeukqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idydjlua.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2npoqyopz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2nnulcuav.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2btdlxkmr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ebqygikn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ulksbvxy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eokznnev.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2gybkyvlt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2itjgttah.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dbxgaoch.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2jzpkabof.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2rhgchezp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdvpnrqb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqpnlact.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ihfitfyy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kwcswccf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2lccwrlhs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2tvakvuzj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkeayfoa.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ehxotofy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ndirazpk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mpmcoskc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2envwwqbg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fekuurkd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ategezkk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2lhabrlew.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eiqeyuud.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2smzzwikd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qihygnnn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uvexbjgk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2pxygkbxw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jxckidyj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fzdxogxz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2inrjvxdr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2iwjsxfxw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2gziptoto.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nlnvtgww.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mshnnfoq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2mvpahkgq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2esiazhoc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fbcjoiyg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eksvcjfv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hfnghrmz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2jzlnyijs.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nzurfdkn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rgabyvva.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2zhextigh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wgifftsh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uwxvlumx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qspblqlp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ebnieoji.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bfuccire.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2htolndbt.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ylpvroph.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ikvqeihi.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2rebjjvnj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mirkfhhr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2vizcmyuw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2uorzivgq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lskhdiyd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2hguuapia.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2rdizhfis.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2bsxquepg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2tavzqehb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ujgpuvhl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2famwqpnk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2newkqhuo.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2sqxfzhjb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vtitfebz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2shdteioh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2lbiccomj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2vlcwskzn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qtjalzne.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2tkikezlj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ygvmewzc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dldajbfs.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cronvksb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kqapmnoa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jjhhvrxd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2gdkjjkhn.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2weqmodfz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2xpcualvj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2aanshjdu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mehlgauk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ghirimhj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bbmvwfxj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lydoxtlc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2gaktincw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tkrwsdce.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fnyrewgp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2crtrqwze.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2zvyulyiv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dmjfxwim.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xvllelab.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nrbpmqvs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kbsxmulp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mqbarear.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2uktqczhm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gxtkoufw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2dfxznhhd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2sazjgdlm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2biaccdyk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2blnlupjr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2sheorrvf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2svjgsbww.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2qbshuvck.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2vntngexr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2klizmbpw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2neqanefa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzmqzamx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2koogxngg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chgehvqb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2cfisggwg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2uzbbcicx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfuiicgn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsktxiaq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpiuuvjq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ortxhxoy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2hydeyygc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2xjduqaiq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2evxganrp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wbtmasqk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2wqqwwcbj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2bkwfhcgt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bvkjdfly.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2fvtaxixd.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnjaczvg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2bshlvjlw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rvcuhzod.html


<!-- 参考信息 -->