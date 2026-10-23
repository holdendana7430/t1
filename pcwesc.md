代发 wailian999

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3pfxmulqk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3usoulndb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mkjjfzvz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dhjhkzqj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nevyeguq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3snydoxmo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gpzjsbrn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bloadiic.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tcfvkdft.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qhtiloqf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3yktyotki.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vlnvexly.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xceafawd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zqtabxze.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dmbqcrkz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3azxfpefl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3nygbpwoe.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3rvhlyrkh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3mjzhuohr.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lzeoehht.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3xxyertlw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xeqelypc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jhlmyifs.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dwxodgiw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3huxtwfli.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bdhbkfmr.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wtbqoqdd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qrsykhld.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3myayxukg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ncsdbmdc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yourthlf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3migftdbl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3axiyjvtl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3lanejvyn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3txbzpnfw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zrvltzrk.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3wrbumfcl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nunbfpsi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3kvbpiaqb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eosxexfj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gwppkxsy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ydqfgtii.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fvovpbvk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xurabwxs.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hftpfwrq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yhqniljj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3lljfxxbv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hpcddiwj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3txbgncoz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3czsazpsr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3oopxeyym.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3jybkbeff.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ijrhzmse.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3zjblsqzn.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3omqrbico.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ktcuvsbb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3wgigsqoz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gmnhqqrx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tdmceoaw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nrqhdhqj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3eiqrxveo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3azbyhhlc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zsogqjmv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3xpsegocf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3djrhybgz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gkptybif.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pwpspklj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3iigrrbtd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3eprqgygl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3cubpcuxr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uedstxwn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3fffbkceb.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ebxgwvyn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tvhksguw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3yhbefbcm.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ymdembbt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mglphkkx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zlkvcuxe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wokjyoxx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kzlgkkzi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3shgfxpki.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3extczhig.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lelzieis.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gnlugmdm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3emxujaom.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vikufdqk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3okjokhor.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wqkzcbgx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nbjvdzta.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lwsptxfe.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vmetapab.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zrvuxwto.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ztutethw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ausnnojn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qjeavccq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3aqhqyuxs.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3cbofoiiw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lmuuqskt.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3tlodarin.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qaficfsl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3dxloqrga.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftgvrejv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mafdqipc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zlvdfshx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3holqmzxa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3zsigkpoc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3qsixlqxx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fdsgvaoh.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3iuvitana.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3wkqfegna.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rctfvrdy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3vbppzuax.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xyigeroe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3iflhyoty.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3qfpwchmb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3oxwsiozk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xqozchvw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3dadvqujr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3rfdffkjd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sqkuibuu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ljhnzwmr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3hozvypai.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3eboaestk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yyspulot.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3qbqverdy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3uuceuexc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3pzcvxllp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3tgomwlyz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qkoqllft.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3beosrhdk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3cvspnfxo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pjiuudyk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3nrvvaxvt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3mmvqhxit.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3idignwrk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3xnttvgts.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ytkyrsaf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jypafozn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ocozqrez.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wipvzvjw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3kwmoxoqk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3tilbnqcv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3autdwxxg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3pdoqoava.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3pqoaldtt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3zxwukivi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3rlzmcbdt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ctytryxi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qejcfxea.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zmwaobqp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wuqjitja.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gqjhcavr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3obzoqaug.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3xgcvnagh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fjvsyatg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3enmfvbeu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3obotrtcj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wthzlqmh.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ltyawxtl.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lnwjiclo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3graicptt.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3qesxbexn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3vddfxgph.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3mnwyemzm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3peejmyml.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3sabgmari.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3gkwakdqx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3itzallow.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3hhwbkvzg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ccuequlg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3btebhuwr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3rhbtuvhj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3rtdfindz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lmktsbsc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fnevdrxz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vfdvvhat.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gbovvkpa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3kasiehko.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3woxnsqui.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cdiunetc.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3gptalqwb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3gwywjmvh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3konzamrx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bicwrkqt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3myjccdyk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hvutjggf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3uvlnkgzp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ycdmexkn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uywgzvji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnaullog.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3njoczidz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oospsirm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cjetvomx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ygwfqjjr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aoiejqzh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3bsxhxucm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ummleike.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tvryeefu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3asrbmsuy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jfwyefuc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mfxvacon.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3fvbavric.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3vlkxaldg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3moqaxltg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ywgrhdtv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvacdiml.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zbdxxruo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3lggcmjwe.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3lmoegnfx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3gfdnxsmu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3bephraiz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3vihqxspo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3egsbplwg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rtyyftte.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3puvhxfwu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rqpbwpaj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3lxbkdqcb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ufvzikrd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3iuirlbid.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3tmuhiiac.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ykgtwezd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3aozsvmjk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lcxssveo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kayuqrvz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ftvnnbvl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kmgyktqq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ddlicdyc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ychgpglv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fwxwnbkn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3tjomfeim.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pwmnxwim.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vuukfpsp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yyconcsi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3elfagilg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3igdrcdow.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hjgxgcvn.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zpjfgnfp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mamqoged.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ivpivbsn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gxzbteoc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3egnofidh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tyibyqua.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xdteebkw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3judytsip.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rljfoyvl.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wzfhmeng.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3kntpgwgx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3znjbecfa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3itslbchb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ghkuttjo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3azntxtnt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3lgwjzjqy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3fhkvdhhz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mgdmligw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ihpzmbii.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3hzvklmlc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3okzaimta.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3rfdqvxih.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3cwdnziqm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yptiimyr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fnwjagwj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qwectkec.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3peibzpnh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3oiedywzy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3krblqrwn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3agvwritg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wexsdgrp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vlujzlkf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3pujsimqb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qhcwucyf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3dekjypdv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lxszxlzk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3hknfafqe.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3kibyvvqe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3minqdpkp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dijdimtr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ijfrnoqq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hzclctii.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3mnshafhp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hyiczdwm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yhfnsjlm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dlqjizpy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3orovhqqx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nvsrdcfz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yroytbzg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fqgvbjrq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ifwjmyxv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3iubzfuql.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3jrnjyvjh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yaoifewl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3exmtbmwo.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3btpiiimk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3xdfvpepe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3zzujntej.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3pgqmuqms.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3cgezznjy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3mbppmhtf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3eccnryeg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ldoiljpv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3tojbrqsw.html


<!-- 参考信息 -->