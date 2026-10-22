代发 wailian999

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2qndpfpgh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2yztnabcx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rtbaenay.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nvlvylwt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pgnrqhia.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oqboytri.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kxspwbkj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2twtwjtvt.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dnqskqmu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bhmubnme.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2gevjepwi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mamrzyth.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bbgkdjxj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2qfnrzzah.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2mzhifnni.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sjrlxtzp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2yacraddl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2btjcwasw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2vwyvresa.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2yspyzcgx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2zavkvhcq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zaaeqcnf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dpjeubta.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jtjgbpqi.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2wrufxgnf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2klietynt.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2tesytcbs.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2hakbhqxz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2okzushzp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xjoccksf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2htmksuac.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qocknbxh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2btduwtjt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2lqseanyt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2relklowo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wyytvikt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2erpsroci.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xnfornja.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2dvefrpyt.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iqtfxyep.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rnpjbtud.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2apanrktv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nzlktphk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kjgabwob.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2egfakkos.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ovrccnxq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rxufaaqo.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bzeurugu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yhasawry.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mmnjbvsd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zugdzeia.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cujdqkok.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2epcotzxx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bgtrzicg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2yosctxvs.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2osvnhsxc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2aajlnskw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lffafkwy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jrzjzskh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2vosfkjox.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2oaswgoyq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kjrbltfr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2cvuwcihz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wlbirmmx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2zdiqyugt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqgunasj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jfzfgizt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2skesdrvk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2icurjgfr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2hgqidqys.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2emobvylz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zuwbcpur.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2wtehwtng.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2abkfaark.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wfnuxdww.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2sfqffzej.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2smrrpnrp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tqjdwqgx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2oxcerose.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2feqrvtsh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nbcczryx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2czicyvps.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2dfnkhnoo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2wsmhinob.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2irbwgbxq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ftntwfps.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2srnlfoqs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lxbkvgwp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2kaogxsov.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xrwipdwz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vumpznqe.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ocvlmixr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2skwamhkt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2viwlmyui.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jbhtewud.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dhqjivji.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2nojyonzn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2afnbpsia.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2qxsdgthu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2itjdkprp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2asrpzdgs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2pmcdyeew.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dlpkfbxq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jyemclfc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2onnlynye.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2efpblhci.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2sbnhvfbk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2adigxmio.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2otgipham.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2obprdnjt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2pdvynqvd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tgwrniiw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tnljkdnz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jaclhgrn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lwhijzzo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2osyjemep.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2cblqfluf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2iliwisbs.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2hdmiflqh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lwovsffv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2rsfzskhy.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qcqgubwk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bfhngwju.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2odtdhsfr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2izjzutei.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xjylbwsg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2bjwytgwh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2exqxfrhg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2uujvdvvn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwbohqsg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2xflpdsah.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzrlupao.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2qerhkbab.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2icalgwzp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2psdsemio.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2titiiijm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2iefsbyjt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2deqhidfo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2joyaopnm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2eatawidy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nzgkicxi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2dluibwmd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qxtaxlin.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nweksnfj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2mpkzizia.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ypgzevro.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uxbismlf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dvplnumo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mgnkowth.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rlwtheiz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2wkbbbofj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xrkrlgiw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rzxxathm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aoibbuat.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2xkzqkkiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uljycqkv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rgrzarrt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2wrlivsxu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wvinjpdd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2wvvwhaid.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fjoyqjiu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2imorhdsm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2lpvivcxh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mkzhsdyv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wysarczr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2tlaxutmu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2bbqcekxt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2kdksjxfh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zwlovvpa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2voqmzsxe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2nrkrzkxb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2kdghzkrb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ezvjwkrh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjvolski.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2nratojkf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zypoelcw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vvwcazgt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lbxdeofs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bwgfqyom.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rwjhggun.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2nsqsvwdo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ovjbukds.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2upwwizok.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2cpgmkaev.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2datvurce.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2jgwzfjia.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lgdjuilt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xujocydl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ejigvtrl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2eihqmhqt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2idronfpv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ehpzznsy.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kffaxthy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2suxepqln.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tqyqdftt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2insyzkgm.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mrvvfrej.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wymfcgvx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2rynvyksf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ifxpjecf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2utivisvi.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2xdydtytn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pykhcwfu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sjuqoupw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2domkrrve.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mnoytblw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wmkqwtjg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hvtgrgsj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jwqlikao.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sewyetyw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2mffypzrw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bwnshkav.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2madudzae.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bazwdrpf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ldbylnzq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2lwkdpodz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2azikvbtr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ysebzgdc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xzpzxgch.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2bfkwieaw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2wemwbyoy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2tbytmamx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bnqlilkg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xcetapxp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gfhnctko.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gfugoeus.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2xgnzaclm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cdunbalv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gqqbqnmq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pqssggzw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zrhshoom.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2sysfalmg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hmjneeht.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vkmvlbhq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2damhfpcs.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2poekpszo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2dnurcqqh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2zozrzigz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kgxwnqxb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2btxgdeoh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hwfpqwmo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cvajtmcu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2jslcjkcp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jgizxein.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jdbvcbfr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wdoohgzq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2uueuavhf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aeplqynb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2dkkwzjcv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rgtkamty.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iayyilqf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gpslsfev.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2eizlkkvw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2queohmpn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2cgrguktb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ritrdnyf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ekiwfovp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2arexlxym.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2uvopmqoe.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2kpzrzbva.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2xnvmixwp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ipdmkeur.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2lwzvfajw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2mfompnxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dyijipsv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2bwryodyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mpvroyzx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2owfusbwr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2wjcabidh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2hhzzhtke.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2obhhiczb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ocjxhitd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2vqdhwuvx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2mzqjagmr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2awctnlzo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqkfubdy.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2xobvpaeh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2fwwbehjj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbdwcswg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjvvfszy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2yentaskg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecrhxear.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hpnauvcd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mzupnide.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgtrlpqq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2fkusuubl.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2rhgafojv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dhpabswq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lsxnouah.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wciojdrm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2mtcoaxrf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2pazjouvw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2beyvasyr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2dpblkycx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ntzjfsdp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vqjngrls.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wkgvismr.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dirvqzeb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wssvygwc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccxifqgb.html


<!-- 参考信息 -->