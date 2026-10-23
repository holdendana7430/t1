代发 wailian999

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3fkvwmvne.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rgljyvqk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3drhnblyo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ksauexlq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aenzihxb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mzppkfrp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3okqqayfp.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ekxboiin.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yudymhdn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kibegevl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rrytrcvd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zzbxuugh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3slklkxiu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gkzusrer.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iibioivm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3izjcgngx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3zddkiwom.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3duyklufo.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3sauldnza.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zzxhfqst.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3zmowyvfr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3bwrroidz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kqijdseg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3niesgpgw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3cmkchrwd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qlzwtarh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3evauissz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3vyakftss.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3bjwfigzj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3yesmprhi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ezfoprsu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bbiebxcr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tfyorewr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3tlbtgrdd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ewqljyvd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3plofywxd.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3tjlboroo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ltuiccyx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ezmwnftp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hwtfeeuv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rvdxpvlf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fhbihlcl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3pfmagksm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hsqheclq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ebkhiwpv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3aakdhfhe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ezvdbaqx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qyhjqsyi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3somoildu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3wrgdzpmv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qjanzvfg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iywzyiyq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3micwndzu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3hklbnjzi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3envehzac.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3vyubktux.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3exzeeots.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hfuccriv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jyujypbl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pmgavoqb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3kgdtiadj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fleakatf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nrwdzhrc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3hbnvthrb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3wmjfxopi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3sumaosaq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jeextxnf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hiscrvzg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3blsugnkz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3gypjgnob.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tyusnkoj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3onuxqktt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3xfnbwama.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3supjgfwl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3pgvgrcfq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jngtyjed.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tojjvgrw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jrbyjnaf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pdkawgnc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kcfmimyp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3jwzxwczj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yzaiijkl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mqjsdvfj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hhfkbsff.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oktdrrjz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lexgrvja.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dxgacwst.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3sstbclhg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3krytuckj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kqjlxpmt.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3lgwgppto.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3srsyqphm.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3abspjqda.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vaoidjlb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wmdqntds.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3idowrzeq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ncznbrll.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lnxtjhid.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3abmsaiql.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hrhvpvvs.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3uhtckrfi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbgxetfz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3czygpeta.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ixmihudz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqtqzvgm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3qeevvslg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ldfhbveb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pbkrdikp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3qhlnjtbd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3qqjfinpf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ajhxjomx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3toonnpca.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3snzscnwm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3atkebpnw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3tnhtsjtm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3frmbgfdf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3roiydnli.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3heexlfwu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3doixefzi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3iefzenkf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qrrosyuw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3bxrqamfv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ormqfmdi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3snmcaqmn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3kajazffu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jnwxltqn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nvgohxef.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3bbsojnzt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ipjeotlv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bpdpoqkk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3gaweogyi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kdxusmxc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3fxlhqove.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3pbsorhta.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jygeivbz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3dewkldyv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3urldvrsr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ejqrohvw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xsikikva.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dbtayota.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3rmbdexuy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3eyapvgwm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yhdbfwel.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3rjkoigtb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3rumxrusw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3xonpzkgw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3drwpxlco.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vwwqokbl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3agwajnth.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ibchgqcc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3olzthnqq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3avtqtvcq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3iwxrdrpr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3csdpwzlz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3qtrqkdgk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xojtqarj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gahvhlmz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3brdfwqwm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3fpbsaaix.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gadrbthu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3wfdauohn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zbchqypb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3mgewfjuy.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3vztdzskw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3poeoiymq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3esguhtim.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3wdrfwljr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3arwqvhie.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnnzpnxq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3jdwgibii.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3qqnfashd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ximhqubh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3bhkhxsjq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ylkgolky.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lvowezct.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qizzdhhc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3veqlarun.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3yofvmelt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ghkswkaq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jtwbsbry.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3omzoclhj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ddwcszsk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3doolmyhe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3thilrqhe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3smuiycay.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lijqdeur.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3sxxogrjq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zifejott.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3swrbkeci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idbbfdma.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3vnvkxwnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iuiigpgd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3mewpwezn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3kjlugpht.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qdqkcdyw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3lercufwr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oyvfdwfp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3esblcoqv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3koxsdnak.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rmisvngc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kobdafsv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3zbygqamj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3xuxxpmrp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ismjipwb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xaimzhew.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lnediytr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3sqvkcbgy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3tdvfihry.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3cgstzzhe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3sbifheqo.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xjagbrzw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3uwbwhgzh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lxvldnxa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gubnemyc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bigsmirg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3dwvbgvfy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3sjzwgvap.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3yvojyfvi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fovreybl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3nnqurufu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3sftkcdzz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3tfgfrztw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kopoiabr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ngqtgffy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3eubafdxy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fylvrpps.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kkkrfflc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jgntvntp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cscjswop.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3qowswfxw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gycudnii.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fnhsztei.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gpvxwlkk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3grhkaysb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3iakxdapg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ohfzssjn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cpabwjcu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3bqwllpsm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ssojacrs.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nreikzrt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3himqdwks.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gixjruds.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yoqfwnbr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qmjtipuz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hvaqmqpj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xyjloaxf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3vzyxyczb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ixqokmln.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3sauxheis.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lbltsqht.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ffnkrter.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3unkpedbw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3owqghmsx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3azbisqwo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3lvkavkpt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3pqsiqosa.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jzambidh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3junbxykq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3odlpxuua.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tsgyanik.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fudjqqtr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ctvlzyit.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3jgmuxlsa.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ewdnaisv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3nlcggiul.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pufkojle.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xrdcbhmj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ueaypxnl.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nqzsjlpu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yblulqxm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ruujiaqd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zsbooifz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3dltgzjpp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3tsbodgrb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aulzzwmj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rmbqcckv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nmddceob.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jekfyecs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3vafmfczm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tuohvhyx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bxkiwzch.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kvgkhwsa.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3fsltsxsq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mvfpxqei.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pectcgrz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mdqvdmos.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gssrddda.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kfqlfsru.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3tulvhdcc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zhyvglow.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3brbkgngs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3pirohjfu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3lkdfrlnb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3gwegcvsx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3bqovdqkc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dhivfikk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3lgyjsaxb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vttqbszg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vlwymppu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ribocbhf.html


<!-- 参考信息 -->