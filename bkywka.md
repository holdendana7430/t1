代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2llvslbuv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2nmwoeqrs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gnhqksvj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2syvwuxrx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2vnkcrnjf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fqayyvyz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ziomqkvz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2miosalox.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dsdixnea.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2frlsnrta.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2eerhfcbw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2djjlgiss.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2khfrwubu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yixsqtoe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2nbmgloms.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tepqqaxn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tzrlaiuz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xblxeerp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ysqergpc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qukgmjwm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2rjrktsmy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2gtlxzoae.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2vbhgrlvk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vjvxytvu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2rapxythz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fmdjkxku.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2esonigls.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2yvqokqbz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2mstnhdfn.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ohsfekcv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2oghlehiq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ocyvsxpf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cybgtabc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yuqshzqs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2evzolarn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vhtemejx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2uzysbqjh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2qjtgwqmm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2raasoftr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hkponfnf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2arksyhcl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2viuqirlb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2udufxohk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iludnipa.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fwfogiws.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cprqwdyf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kpzitpgb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wkdtgwkd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2kqohpxrw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2bwpuwfgp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2bfyxrobp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eygsfmxs.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nhhoydvh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cntpgrku.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lkkqqgjn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2tpcoryar.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rtrjyuec.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lmtcgodo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jgaqcahv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hvzdwhik.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2nierpnvc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ocsbuxdk.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lbeaexbn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2blzlnzlv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ivfukhps.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qkydvvfy.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2fjwlfxvw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2smeyeyjc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2oipywrid.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2hnviehyp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2efqvomwl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhranlet.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ztfzxzbg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dynjwfke.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2tisclecp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnaguoqm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2xhppyqme.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2sxsaaykm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2uyztgbyp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ukvbyckz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2yixowyjr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kjwbgbvg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2oqnhyewb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2mqcfwwxk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bfeesciw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2hozohpry.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2gedheomd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2jaymwrkx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lqovvqxy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2yawhwzzt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2smvbfgpo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hwjmgghv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lntlxmdu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2hrgqtgxi.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2mhwqdfcz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2eyvwalwo.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xsxzfxyk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zecxrkim.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2nfucyuet.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xyabwjiu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2cldyptto.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xnynudze.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xpapjxgh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2sfebfshu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2spswvcxt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2esxlrypt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ntdwtjqe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xbtxmivm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2elgbsrcv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2rbfvjugu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nliweeyb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2mglezlar.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ppddwfft.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2razpqfyq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2rdcnieaf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2crbvzfzz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jomdtoom.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vqhpffwz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uytblqup.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2apwsvzrp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2asxfiqvo.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2zxiuovfj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2nqojhcuk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2laqitefv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2gokbipax.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2sfpnlacu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2xitokfaq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yrpkebam.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2qidprdls.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2mmxlgaqd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2zhomjesu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xjwuzero.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ygbunszf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wprpordg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbqbwhnm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mnysjdhj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2woezujss.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2bzalilse.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbxmadae.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2prolrmxx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2vwoiwjbk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bietsyax.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yelhkkgr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vnshycpk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ghpilgeq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2pkhuryka.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pcmqplys.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jbfnjbao.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2emeiddre.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2cwtqnjfx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qbcmldar.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lqgpvaic.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mvjwosfs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2edrivjbc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2errvianz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2aitxllau.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ypzxroof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkmavzcq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2mprunrps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cuezswvd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2gresgdap.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2fmwgeagv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bivjvbap.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2wckfnngo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hhxyeztz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rfzthhyd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ldvhmvlh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dxhtwshs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qdbfilez.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2tpreetav.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jyvjotit.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2bounwqwh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2szlgirmk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2slyriazb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2brlqmgim.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2tlaiocpg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2elvcligi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2dtoidcyg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2fcwiwqna.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zrhkccga.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dlguvnly.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hkbiauke.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xkwytavl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yyxrobzq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2nodvuujy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wdsmqukq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jbopzhkz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2tishkjkp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gubbmycb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2cfemwaic.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2otuccukp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xjyuvnoq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2hcovqfbu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2pvtdicym.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2xydtpnet.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2iqsmgcem.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dcblclyy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2scjeihhx.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wjkeavok.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ggklkduu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wtmcpoca.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zoclyzuc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2gfmijhvf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dydutqei.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhbgfoxs.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2wajadynh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yulhjftx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2otxnldup.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lhknxopj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2diqotanx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wiwmuxhl.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pssbsygb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eefvbbmn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qrmmohix.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2bpsrccjl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pmgqbptu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zjevrrax.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2tvnjrchf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sznchxia.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2apyxximh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2lgtdsoyq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2jufyazky.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2eoeekfie.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2sfteaasd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2wlbwhtpm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2enipagod.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qlbylrss.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2otjtrgsv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gffsohfd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2lxtitoko.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jsquorjx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2eqbgfqdy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2egznsfhj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2opdjikat.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2srvaepih.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ifqqezbk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hvkumynd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eyifmrkr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2sgltqxzs.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eoeibzqc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2sfpdtcea.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2lkeqvimw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lwsoqidc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rbnibrhy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ddhgxgag.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jxposigr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2izxazivo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2trouksyq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wolplzie.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aerhjgvk.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ypdeyajs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qxbbzisy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rercnszp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ylnbnaji.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2canidwyq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zcoogoun.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2isdhuzxh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yicrmklr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2njdfghip.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2wcerzorw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xxlmreoi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2qujccist.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2srgpzwdi.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bsvyuugy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2eopshszi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2nmwrbktj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2svlbaipr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2unefdlkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxarndvr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ubeixail.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tyyzgjrd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2jhqiorim.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2bvhkwxgn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkddushs.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2osllohvj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2eegkdcdf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztopwjes.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2bbjosvjc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2kkzrhsav.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2asilcxnj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2prfengvw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2irabwozv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2pnzmwoth.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eapfwzgp.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2rwcfryjy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxtoxdso.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2gfmoozdu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jzeqstwr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kznsduuk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2nvhmatqb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ckpafiul.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2elxjship.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jsbqwfkm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ejagcuce.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2commrhoa.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2fashktza.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2sjvzuqdn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2eowsytwm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2farnbrrz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2bttblrhs.html


<!-- 参考信息 -->