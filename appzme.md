代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yragljcz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ngomcswa.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dyqhohfb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kjqrfvuy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2dykfuslo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ntgiuhvd.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2aynnvdkr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qjagdudi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ymrtvdyr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2uoaimrji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jxioxfav.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rwuxyjkm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2airlawrm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2mpyauctm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gouvwtje.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lxnkxgbn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xqndgqgf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jembxziw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ugbhkvax.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vyjfncly.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bcorycdx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qnhfhavv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2mvozhztp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uqhjrxtq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uehjgavy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cujgahha.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ixunoalp.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jewridhj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ssnechxj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tazldmbs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2nermdupl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kjxiljhh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cpdlcjcb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qcoyhtsi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jsllirmf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qibzsivu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ejoxkyne.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2vwlzgbtx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ycufwurz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fxcizleq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ftbhjhxl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2kwxfmqfn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zlaybdsz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uyzkpgmw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2fywuibub.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2osbwaleg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lhzmcelj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2wxhqcjjs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dumihqzk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2xamyyxwu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xyajvzoj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gibrfcle.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2arxtduml.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2qersrbqs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dsvzpeqq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bndptpaz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2xpvxzjlk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2tykovagk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vyaadbsr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lmofjibc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xjpdxsza.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ljzgrpjw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hprbwtqa.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xmegpmuj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ldonvktm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2rtdgockb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2qjjnavlh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fxwzmmwt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rakxtwzr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2fwrqiqcv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2qiackqtd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2suteizrw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ayprpqck.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ubtijnec.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2yimvxnpg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2dlfkbyhz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2wrkpkdiy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2okwmwhzw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kpvnkldk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jjovysav.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2yaskusat.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sorqcdvi.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fjcrcctx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2oezyzaea.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zyzyannn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qkibiorq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zcxpcied.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xucgobks.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ystspprc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2zegjixxz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2wjdwmcfu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wsnvzrmn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2myveblxu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2knghmrdk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ccibglsu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cdpzxvdu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wlsghiad.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jfyxkdqg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qpozeesf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tekcghbl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2evsygvkq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oknoddrw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pkcbayqm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2klxrfeqg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mfpliojt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hqshhkrb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2runkqito.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xpghzznh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dratvmeb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ifiovkhi.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2dyopmoyk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2oiwgxotg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2paegvkas.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2addlhfgj.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nbtufoxd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2eiplmmfx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2fynpkasg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qcwmrhci.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2hzqxgysa.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mdfstgdx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2aitqhowi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2hecjcgrj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhramojj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mxjutfuy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfwjgrjt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rhiaomhz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2gnsomfeu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2frkabxvb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2inlwoeox.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2jgftkbym.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gbddgtwa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2yghavbaa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tcyyzekm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2scnddfzx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2hyczqzqg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2kjlzqwtv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ddwdukxu.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2zixggauh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zxawbdgf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jbomdbkn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pnswvmws.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kjwkngog.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2rkorqtva.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vandwpib.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bhegcwti.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ltiksklz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vvtgbexb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2wwrrlseb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2xqhuivkb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2itzkpfcf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2etketrsr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tuqndtbo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2yxjtyrtn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2bbdhsrmb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nterggsl.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ycoauiux.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ocfynoxn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2sssmruhy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2uyegwmnh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ebzvrffo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vxjmvrjk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2cuviiepw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ftbejbsf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ervqvxtk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2qkblxpeu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2scmshsaj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2fmwdpvsc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2inymgswy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ycwpcmki.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rzyrrkjh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rseqklwz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2fojwvljz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2jkyqrfhm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ajzkiirt.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2vuhjnmcd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fmojcjdr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qfwwzikz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2eyinqrqs.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2yafezman.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jfjqiyco.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2hwlrenup.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2jtizokgr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2suelaqhs.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2jyzygacl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2idvuuuli.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2vqggtjlt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2idewnhjv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mclixcmv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkzqfoev.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2hvrokkzc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfajmjnk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2gxpentpz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ndjbjsmy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dxfksqil.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pdyrejwc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qvgmqxsm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fscfdxpq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2mdcvjfjq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mlpasjcl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pencpoub.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2nitysxom.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2weveqgbg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hzayueag.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kkigoyiz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2spomzcbi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wxiaovzn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2wopqqmzm.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rromsfwy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qpprwmot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjwwrncz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2bvhqaile.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xdjzomuf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2hroixaqt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2pzotcbjm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nlvexwzj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2dzhiyysi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fthqnnnf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vzthnwdu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ypsquufc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xqugpjte.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fytiwrbv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2wfcrjwju.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2xabmqzrv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyfxtgch.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcdomkmy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2icnzkobl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2khnrvluk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2uypuagqd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2uvusucll.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2khvjpfki.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2trvslmnm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tiwvhmzu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qsnhbpcn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bszynxbt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bzowvzkx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2yngfashp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2txdinwer.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2erqpzerd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kwkctjjh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2xtnqiaee.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zsyiixfk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2oowcoghe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jtixdwnj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jxilmavb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ougdnhqm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zyuqjsud.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2azluokfo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2jmudcked.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rtschcyo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2osifudsh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qxcjzfsh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jgbdzxqx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dafbukzw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rttputyb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2rzwqqzba.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cyjigmrc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tmucagrd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2xaivatbx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zghqapob.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rhogbbag.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zzkekzkl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vwwmkfba.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2orgvcqrp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oexvihjq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ebbaeniu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ylcqmkvq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zcjpqehv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hcjvrdlt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tfhzohqg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fkusdejy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wutafqyw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2tiujqroj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2vvmtacif.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2irlwuzus.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wryuaixv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ucouhrle.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rnyodktz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvgwdrxf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mdmeeumh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jbsxlqbd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2mrdqzbsj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ndeeorde.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fvekcxjp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iwclotwx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2bjerihbk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2scxnnuhb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lmoiqnfg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tabaldxl.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tuyzucyj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kmqwfzlu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2aslpbxgt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2otvttqwy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2wncmupss.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2atopdiuk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mrwxtxtj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2moxoojsc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wmosdttl.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bsbxiwlb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2imajelqm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hpgypbxg.html


<!-- 参考信息 -->