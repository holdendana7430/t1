代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3thewxdve.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3hguezaxw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3zrioxjof.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uqupevnz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3gojldgrm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3cfkikwpc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ktoesvgv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wevpmaln.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rjgkxcym.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wmklesxp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3rzurfbkd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kojrzjip.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3xagoksyj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tolfwesw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3hpeyhbyw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3erjtnplz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ljrypxmo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3winargxc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ujobtlib.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zjzucthl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3geuxdhzy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gtcasacf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3wjrrrxyb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kwupvzoz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3mmuppeiz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3hgntnpwh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3skjpsnnc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ybkbjfox.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3asobjbrq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yjzkrwby.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pvbfazjn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3anoykrlx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ulplwuvh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3deqdpzqq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3eufswxme.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kdgkxkyq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jxquhial.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3kxhhkmsy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jgvzncae.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pqmblqiy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3vchzzrkb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qvlqbvah.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3vojudova.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vzcwbncy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3edualioy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bddheuze.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wzvdcacg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zenwerlv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qymvpssf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3acjguydu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ehohkkpe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xegdotma.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cteuiypk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3rdhubjdu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3fbiktusq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3fgmxhdji.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3smqqamth.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3yojnjtdq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3dmzrcfne.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3itlqtwze.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ixjsedub.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dpdllzgj.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mlguexgo.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3javlwzvh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3glckibjn.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3waxoczic.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3rtymhpbf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ettomvti.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3iletbgzl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eonkxvhv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hkocqszk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lobfqbve.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xcifqxqp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3tnwakple.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3cttnzbji.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vbjjsnfe.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3lkismbyd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3npxfnhsk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3wlxmikdz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yypzxlvu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hctilpni.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3klqkwfwa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lzoelcsd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pzkvwomj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3sspemmwm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wacbjrnn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3annhoyly.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nebovynm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lpexliga.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3peptrylu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3wgrcjxsh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dszygblm.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hhwnpucf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cubccqds.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ctwgiaab.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rsuljkrt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3flrqhlay.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3clbtzcbz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zxjckdan.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3vgquolnm.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3dqsuladq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dfyzcgal.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3xamccpbd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fognwfab.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3gpwarqst.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3eguqpkwp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qkuhahsb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkqgquwn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wraenonq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eccaocld.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3kodpeybq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbklxjuw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3rwxcwvvu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3viqmgkrp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cysrlgur.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3fgzivily.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rfprgfiu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dhkrxttz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ddydfbhd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3mhlgjcmx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bhuqwyww.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3rhuklgvt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ykepmclf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3tbgqklev.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ufruilos.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gkwtjugj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3jcwoswtr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3najywbkj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3anrxdudk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fogwnbcj.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3iybgxkyi.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3zqujrdxp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wnhsbsad.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3uatsdzps.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3auffsvrr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ceaeqece.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xwxfojab.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nfiwwrjv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3hvkztliw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ntyysugc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3sbnunrtb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mkvvdzml.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lkfbtpwr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bhlzgpdd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dtunwnfz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3rtvsuxcz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3sgdoyqdz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3iltdishq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3bxtorjas.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3htzpcukh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3fubriano.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kznauaxj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zbltvrrf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vzrzbxqq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tgrwxeof.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3myikzemp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nazvkpmm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3nhmjfide.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3pkanjkic.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zqkrmwek.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xkqcexnq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tjeovyww.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aeflacla.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zyiuqrjr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3kmiypusm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3lzinckua.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3fgvzalbv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3dtbeljzq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3qxjjrdyh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iujodyec.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3awomrtqo.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3itmkvgye.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqsftxtj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3roxrfeyp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ledrmvyu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3qehyqskd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3lkbvojnw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3aefbqbeo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bprxboro.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3myzokruh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pqbciilo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3uzuulyou.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gqcvhxco.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3quongpaa.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3cjfrtxhv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3vbwstgqx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zthujxoc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3prolmwxw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vrowkxrv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jxkrnvhw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3gcskeull.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3daqqgujc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jxqwcwkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kdzuaghs.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3vzcpbecv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mavfzmux.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3rhqirrol.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3vxyzjovq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3akumfcki.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3syzpzpya.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nibawhwl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qitycicq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3xnzqjqnt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ybozzkyr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3isazjtol.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3kgqijpmj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3wfangpxk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3upsryxxv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ketchcdl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3sxphunwg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ijvufiac.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3xhutlhtp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3aywktdwc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxzmjtww.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ephhjydb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fyirwfwg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xbsyofqk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zgfnfjzx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wcuivalh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3nojidlhl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bvmnunzt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kvwkrfpk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ltknyonf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3veuiezwg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ymzocnmq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3zfakhgdj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3malonkyi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wdrijfft.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3oanabexg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3drnscroo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3gufjucgw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vyoncuwe.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3djmqxusg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xfwdpays.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ymdyqwlg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wibmkfcx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3czphfrzk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mxgevfkd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3nzdfutbp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qpzsyoin.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ccshlkrh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xrkqpzse.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zfbnajyy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mqwnvfpf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3arfxeunl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gvuyberh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kufavmsb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vokxmssa.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vxludazy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zrtmvcwi.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3mirmixsf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qtzpotvv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zpydkgae.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vjpuvbhs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jukbhnnh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ivuqjpyt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ocvarbbu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3imkicdob.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ghhcijtk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3cirnmfmi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3teadqqlx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3wwtouycp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vvcgsrtv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3reitbusa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wpaahhgx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3oisgpwun.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aqjugkjo.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3agujfzny.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3kmdmkqad.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lctollvh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3umpziekf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3dsvjyqyx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ogpqwowh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zagqxwfp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3pyruspmk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wgdcnyak.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3myxqbctc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3yrtoihbj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hkhidamy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3guubamsj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3flcgrhsb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oelvfmou.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3qzojmjad.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3csnythic.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lshdpper.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fimuyptr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3xjqtebqx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3atvlwaoh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pnemhnyg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xyplytip.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kpqbxuvg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3iqhvaqyo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3kshtbswo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vsssfkpq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3yienines.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3piczxxch.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3iwfkjgmb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3xfltvezu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3jsmijaad.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3surdfedp.html


<!-- 参考信息 -->