代发 wailian999

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vgtefqgg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2uaqwzyrd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gjohrflf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nhgctpew.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yhcqlgip.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lbvltsrq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2nxweryqj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lqtjvhuo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2fmtzkagv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xmwjyejh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2idprmsue.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lepjjkkb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qkjxcxmn.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nsssabfl.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dopnqgys.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fpmdrexo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2hmghvukf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xsxoptmh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2dsrgylii.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rpmfnssc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2lhqenpma.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2bmydisgz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zaygzrcn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ipdbwral.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2frpjmmhs.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ubdaxeyj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vsiayudy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2afgyrnlk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2qlgoqxrp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2anrkspub.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kiukrlwq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2bfcsywdi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dddtbnoj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2vrggkpll.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ifemlcoa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2madeshun.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2msgxqxvo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fcxqmwln.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2dbywzayw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2worumzkx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2finwelhn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eurbcqol.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2iiwupqhm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zjugcbni.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zelhbmon.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mnsquycx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2vgikqixh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ilefkzqx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2oiiuchjc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2kwoaqext.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2zhhpaeqd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2woetejqv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2qbjfonmh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2sxsopsys.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2iwqjpkru.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ntigebcx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2taztfbvu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cdouxbnw.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2frnivndm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2tvvwwgsl.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2txkagvef.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2emlkmwxn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2iqsfusuz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2jkshracy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wadqzfmc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2osavlpeb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zjsgdigt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ppckmufp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2exbmmqye.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2gzlnleoy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2oyqiyiuz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wubursos.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2nsxfhqsc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hxcvxcwb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2lheamwhb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2oiarzouw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eycgxnkt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cyhauwhc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jegxgylm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jwvhrftj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2mqrwdpmj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2mzsespvw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2sxzcmvpm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2laequcmf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vzewfpzz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fbnolzfb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2baymybde.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vrbuhloe.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2huwxayck.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rsmbstud.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vuqqmrya.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2khcatqfh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2viielefi.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ceerrzko.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jtgfhyvt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2hkfjzajy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2antzflzv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mjcfqifk.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2unlhtutb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ntfhnqzj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2voesfrpj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2tctrdtmd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rtxpyrpp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2likgecuh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gdinzkqn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ennmarzq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yiooedhb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2splitjxm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2wcsxjery.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2kebiklty.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2hbxcxxnn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2qcfemfop.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xraxntuw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fofmrwuc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2eqcinlhp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2huxcydps.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lsxdtbzk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2zcmtjmln.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2mqjjaqut.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eqztubjf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ahzdyres.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ifmyakpl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2kzvycmyd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nhhhwbfq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2xywsvedm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pnrwcoly.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rhxtqlsy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2whucrehs.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2lfsecrrc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2rzpkjbgl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tkecmlod.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2sfqcgtvv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ausasvkb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2tzqhdfum.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ccjwomyx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2eljcgmqh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jkoxfklo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2zjhkqmtl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uxzmdchj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jcxkddvj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2swknlvui.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2oeedzwjk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zrjmygbx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2zoergoqu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2rknwtwwz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2sqnkkbwm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2sqrxcfky.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rdtkgdlv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cbakutaj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ywsiikqp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yewimljr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2psaswyjs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2nossmsim.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2jbxrbwtn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2nvrehlis.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2usigtaye.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pouigzov.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jjlyzocp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eisajazu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2kycnakzf.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2mgpmfife.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2qkbytonc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2hglsgjsr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2zaqsqdsd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2tdrgmimk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dapyqvsb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2kpeowehb.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hwdptmag.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2fvrkwipw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2bfdvezty.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ugwpmjbh.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2eoekvasn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ubncaqkq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jdccuwpp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lembuzyp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ojfsxrcm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2saictidy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2fwzwvtdm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lhconwkp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ltefltlf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2vlfiknqu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2buvodduh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iimexpkq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ntdjzghe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qaebdfze.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ktobizlz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2txwhzdfh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fekpudia.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vpfpvmjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffhegsln.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2bxxmstcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gexhtlgz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vvdoesos.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2dpxitcaa.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2noemwfdz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2tcnrbjqq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pewylxbm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2apyigowd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2zfzvytah.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yrrbqxkk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lhyzfdez.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2awvhkhlf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ubdadqar.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2tjrfuhty.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2evczigba.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cezbimsi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2aicvfmrf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2mltmlkkf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2lrbvydqh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2deadhebh.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jreouwwp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2brmlsmzj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2czxdwbqj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tqrjmcgo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2auxiurdd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2dcydixag.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2mecmddhy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2oqensdud.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xffjyfgj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ivjsawde.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2impbcbwt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2piqncfem.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2szwpsunl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fpnomfqm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2pbdwcyju.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mgxdwnov.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2hltuxytr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ygmozsli.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2eqvoizsf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2dvgilvrg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2riktsfmz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zijpzofh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rlmdxfsh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2abrohbip.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2dfoxidcj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ywgnnxuu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pubdixnd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2reqyddkk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ieivwaej.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ftsdmiuk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nmstosos.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2adpulsdd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vxmrnhxw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bffvddnv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wsdsclqb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yrpnwthu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2xnxtpiwg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xdwlxnqx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2umxkjdrl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2spoeyond.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mslrjics.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2iabdrqic.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2lhjjahlq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2viyalszt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2dlhalmhr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2vtyfwrkv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2sxhobwno.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2kcdpogzh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rpcjzjax.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xfwxbkuo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ijmlhrbb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2wlarzijq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qicftxoy.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2rprwjxmg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2wufjfrnd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jwrpnytt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cdrepahd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ggeqdttl.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hmotefbm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bapwbfpd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2cibcrzpd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2elziqngb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2bcprwifi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qvxgprri.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qwdnjxrd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mgddyzoc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2umfgqgmr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qmahcqgw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2cmmgjuom.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2quyizfwr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gbkghovu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ssmgwukl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2acfgfclv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gnnghphc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mwzhwexf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2axvrdjiw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xswombql.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vjbsahdb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ggokfbkt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ftvfzpwp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ppxlscur.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2djnyjpkt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2mqngearq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2tocyuskz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2xdpqwnbi.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2unomwyhm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2xksddjnk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2pnxfvdoa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ywugpngy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2yvoejdkx.html


<!-- 参考信息 -->