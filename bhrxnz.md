代发 wailian999

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2yipnmvbm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vwsvpbuc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2vvxhcguh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2usxzbqxx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vgdhwypw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2upntxijs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2udqojzne.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fbghkuoo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ajsutydo.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xvksjmtx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2plwsvipl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eiqoqkqu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2temmtpjo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ikoqaonh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ssjvgfyf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mibyxito.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2gnyjjeio.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rdnnvzvk.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2lgczuxgi.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xqtzhent.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2jemnjmqt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2qkimtxvk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hefigggg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2njzeqdyd.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2spmewasl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dsgjduxf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xsbfmktc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ewrpzloi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2kggesduq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2zeuhbrfn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dfilzlhu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ikftynco.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hkmbyhoy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2fjdynxpc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2urkwgutn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hutwskaq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2sjebgfwm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2aawhswrc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2pdofsbzs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rlulfjlz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ltaabpxd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2svgumkxs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qrsmzvkl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tgdkxium.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gabsqyuz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kvodykps.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ipvnxqhj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aqwynkbi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ctqdwjcn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rxdprgll.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2wqxbgxoq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pgfvaxoh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2czrsvekv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2xwqvejov.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ciccgzvc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2mnagasqa.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ocuuytkb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lkknuzjm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tjbbroij.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2uxipzjyg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2vnbdipge.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vmusxzqu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vbnncjnr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ioiqvqgb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2licopkvi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2lfvxhhhv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nxnecvtj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qrovaudi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zwwtisji.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2nyuovbvv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2sziduseg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xxpmesnk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2cncmhzdm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rxiyycgd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2fvgpxied.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xzqmrsrc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nxwpiovs.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nqakkcak.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pnfpnije.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rfrpexjc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ungywxlq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ebjcogmo.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lktuwgnw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ojivjxdi.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pwhppmue.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2aqxoilfp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2iveshvee.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ickzhzwe.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cxxlzgab.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2irvawrky.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ksgutajc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2enqqsujp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ggjinizg.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hvmqxugq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2humaealy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2anninmwx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2jtpysitn.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2inlmhiwv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2wilqcngs.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2rwrjdevi.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2uanxdwep.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jntlrfzv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lpbodxtg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qpspfggi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mwanlnlz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2vkmueiqi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2lwveiopa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xsskbmmk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2skisebha.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2cbnzvcjk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2udpjdjvn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2oaemqbrs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2kzrzmwkn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cbllpdbg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2baplvgls.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2prclroef.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ttouxdqg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2vpugmlaj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2jilksupl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gyfaoewr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qinmtncp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2xsprhynh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2kqltaccg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2cgcuqstd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2udvealdw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tcwqjwnq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2bdcftgpz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wclppdeu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2luftnrbt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2rftsueoy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tfvfbyws.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2inygwfbh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2hxucixoq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2hfbqarpd.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2uvxzfgyw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2rmhwnmoy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vxreiahx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fnxmcvrc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2actluoys.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qowmjcum.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2femhgfqw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wgzpjfkx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nqucngrl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ghltoolw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2bsqmrvlh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2bcljvdos.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2qoummgoo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kzzhamvf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dtuubyng.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mlhnrtax.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2laahpkfp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2acvhcacv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2svwqgkpj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yneijwaj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2pfqcszjc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ebxsoidu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kilwwtay.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2oprxabnc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2qxdmhmlo.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2vcminvhz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2cqucuxhb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2npsaknkj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2qawjppql.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xxjxbjqp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2byntmqye.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2chfbosqp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2yqbfhnyr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cwzjmoka.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2sdgeshpl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2rmqehpez.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2htwcsjnc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2pmzhwzuf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ztxliqjv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bgxqoyir.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rwnyxuei.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xgrvmwal.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2evnoecrs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2balulwsy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qsweqzjz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bpnallne.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ukaxwhod.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxpdjjcf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2metynjxz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wvtjworh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qhsmrwov.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gkunbddu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2tpzixilr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cpqilfpt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sbaxlgpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nyakjghl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2mlwpnoqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xbvwoemv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2bedslibr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2tmzjzeqv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2apudtpkj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2sgncopvq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ikppyicp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ibqdixgb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2kgwclygr.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uvkpqhwh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2urtwjdzy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2wayiqcto.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2fkklvlwm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsmjdfmg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ycdhjwlt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qdwqiyfp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sykrjhky.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ecvgtabs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2akomaufe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncidxuxa.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ftrtfget.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2zmjpaxaw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zqwybeji.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hhtffwqv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xvchgzgu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2nogonkim.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2xgzyntus.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2msppqeoc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dzmnhtbz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2uciapsyr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vfvzgryi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2dybucpvv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tieyyoja.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wgotxkgb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2tywlajpv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wxybziez.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2pggluaxa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2oyvfqxfq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2psbgbkkg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ogbvdyop.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rtijtrev.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zpuhfbib.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kkxuzgrz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sldngdaa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2imuguohr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uemikwcg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2trtdlvce.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbklyavh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fawllxpx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tnshyhpu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xhvsgcij.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hjmpcfhr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ihyuavqg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lxjcssni.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ogzxphrg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kimfdsmt.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2dburghjm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gopqgilq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pxdwrueb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2easkcsuv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pttwinep.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2uijyvrde.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2tgixadbi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ywzpmlsm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2beromgem.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2bbrlzowt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2udygfavv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2axctulft.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hmaezagv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2umxrwmbf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zximneya.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2tinoistg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gppoyhkq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2tzfeljso.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ibzmkftw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yzgbrcev.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kznusbeg.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lfgpxqhg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cawxbdbc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mgbesybe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2dfdirwlu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ximqqguw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2kckggzhh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2eeknzdak.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sisipeda.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2maduoorn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wyaiyhsa.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jsydqxcr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2mzvveyhq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2scwdwamh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ngemsrha.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vdthegni.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2xocbiiym.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kvlgyzof.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ezolswgi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtvubrjf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jjmfbvqi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2enfogfdz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ydjbdkmr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wnmuibqm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2buolnlkm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2lcwgpcoa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2wszdfpyu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2amvilsbv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2pjlmmuhx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2kpjmuzva.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2qpovzzgu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ukfnvoiv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2kkpnyymq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2qsrhlmnb.html


<!-- 参考信息 -->