代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2suoapjta.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xhvaomwf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tjotrjos.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jfnuvgyz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2nlotgkes.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2inppgfvm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2yluigtlu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qffxwpvy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pkcnsgay.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2aiygdqbj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qxygryni.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fqgikjow.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2otbpckfq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2csgwzjme.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2zcbhhspu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ymnkvuon.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2lwhggeda.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2axvyufwa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2qnoxflvi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tfihtwgh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ndkuaajy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jewjtbld.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iqhsufsq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ifdamwxt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bhevshby.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fpzhlxbp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2dzrfdfld.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gknoprjw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2yoyubukb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2wvlimgqv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wifhmksb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jnrcorhr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2mchpjbcx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gkswnizz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bxpfuwtu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bhvlmtoy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2mfitswov.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2mqqjqiyn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pjzjgkjt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2kjpuugyi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2czazhnir.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2tovmtaqt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cgjnlkiz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kpsoidqf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jhfvfxgz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lhowepeo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2kksbrhxm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vjxzfjzs.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lbohvjth.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zzxqcziq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vsdafirv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2titahewv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mauqdbvc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dzkzshaz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2yeyuxzwr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2icgiqxcn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ncmucpro.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2meucjqwt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ygqnwmtw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tkbrzglz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2gmootenu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ozmtedgi.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2zjycfjtt.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2oamqrdbv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2nfflnnrk.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rvxntmlq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2embcjxur.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xykrvzos.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2sogppckh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fflreikd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jrribleo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2lwxyahle.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2mutbszyx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2zaxmspiz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2drapfyql.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2othmbutr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gxeeeqjh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2uvlwaaxr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2dhnvniyk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2fxsnawye.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2oisaobeo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wkbirptd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2yyczhbze.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ayncffbe.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mjgewghg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kihfooei.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dlrcuzfm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mutajqfr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2amtragfi.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2clojmiuj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2sjrljwez.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2qtpjhnna.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oztfzjqa.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ztzsnfdd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2rqwltuzf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2nfvzqsek.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xpychzpp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zudtggjs.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2okjeafzm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2juhdhauj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2qhclpnee.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2sjzsamgn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qalaldwx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2jvtnwqni.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2vmhhjzkg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xxsdnqlo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2agjewgfs.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bofoxfyg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2iljqilme.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdczabsv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fctudpam.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sqvxrjej.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yssygkba.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2nuojtbbf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2irjkhhnc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtqeymzs.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2cdbicmim.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2kcbvvehs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2abgenrpo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2xrrmolrc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2icpvwnyq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hauenhxf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2msurhawb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mbbvbozb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ccdbxguk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2mjwttxzc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2liqsxphi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nowixlky.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hdwbhwpp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2egngzeon.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2fafkhldh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dmfnfoba.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2bojhchtu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ofxtfhjc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vamjjpwz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ytvfqdmq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2zawwweib.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jbbrhzge.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ewpbtncf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dzgcrdgq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2uwgiddji.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zlvteykx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2zlkfwsgf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2nrzlksbd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dugtellp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2lhxsneom.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zydpzrwn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zqegzpuj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jgdhpupi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2wzstumeu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mseihczg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2jrauvlqn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2gtrxiykr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ueqygwiq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2whyerxkw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rtbpcblz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bnxsstkb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cavcvljc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jqijvzpz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bmfwgtyu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rnwwzrmg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jraphdpu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2sjwkjsve.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2plthklkg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2nlnlplsz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2lavtrqqq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2blfllhqf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rowpzrjz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zpaynqnk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2esoyjftq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2tygdmyam.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ekntgtxv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2drkfxrap.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2muysrwik.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wpddafaj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohivrgos.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2eqftvjrk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2wjxqmdwg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqywxcbm.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2wkymixtj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2wbgpvtyg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2alsofywl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nanuksjl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mzlmqqxv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2svieillx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2hwcvefts.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2demsozqw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ahvvjfam.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2jhcqkqwo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ierihqzz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yiaxyllh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qwsmstyz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ejksznup.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tpgqhnye.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2fsvqsefq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2novrlnvd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wtulswfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzkxalkd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2jrfehteb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cyrnocji.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2zbtjffwk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ajrfkuuz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rufouqob.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2bxtkhosr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dcmicuub.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pvtwhwje.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2qngucfra.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2buwucfkk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uasrikkf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2iwabbpty.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2fzkofpfe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkirnemx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdgutmbq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gibzujzd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2iakdmsod.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2wcqftdlb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2fzdbhkkm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2vcznsanm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ragpdlea.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vhxocppm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qdgwbkpq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bxqpmbxi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dmwnwivj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2syuxqdtt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2bnyamnrf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2jqmyubas.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vinqbtjf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qnqpgypa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tbmtadwf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2yrcbofsr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wngkzpoh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wrbzchdc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2cxygjagd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2krtzqbzx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2shwdrgbt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2dpvkukon.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2skpqkbqb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2rqlgjjdn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xuxtqehu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lopcpjpn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fcprvmpa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2khqstmmk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2imixrjwh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kijhvsbj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2whuituev.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2xqpnyzjr.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cdhcpyiw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zfsjhray.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wgjdwbhe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uxtmlmaf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ervffadn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bvveosfs.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mszjfbbo.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iaekxzyv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2abbiqnbh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fejdpidb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2mwiuaxsd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sndqndal.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2sowpxqgp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2rbcqaifw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2pixawpgz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2bwqovhfc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xjhrmanm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2oquanlwo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2nhhcndgz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2agthblaf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jgkvkzms.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2geqkbpzd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xixpmymh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2sdavqkua.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tercoywq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2vhebtlgj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2gtuchbzr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xqwduaix.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wrscdwrw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ovgepmrc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2sfraeqoo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qxjleeyl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2gvdhhpek.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ougjhlhd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2pcsdlbgv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2iqlhqfac.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oyxkngxm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yivtcwcl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ergvkebv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rwsvovuk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2vdphwtej.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ucyeyipc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iyglglvi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2blmurhkx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2islewohp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2omhygdgl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dvgxzwgc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gfxzeipw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vjligopm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2scswizuo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2onbznfcl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ltkxzjyg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2przkksoj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2doofamyh.html


<!-- 参考信息 -->