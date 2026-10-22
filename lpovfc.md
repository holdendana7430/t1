代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2sgrishtp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2isoxwige.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2iqwvnkng.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bnolbucl.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2zwdqolul.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2flqdifjr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qggfouts.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2sjhgfkeq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ewmrxlok.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ckrwuwdb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cmtppxes.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wlzueqce.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2rfwozhrv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pdtnubhf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ylciedkj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mgdyydti.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2akdqkjnd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tueyqkud.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zewvzdtz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jqjaqlbb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2atngbevq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xmcqzygy.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2hhrpqrka.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tvzuqfnw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2tsgwmotv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2cxlkcfnu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ggthggwf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2seowrffo.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ucymsghn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2raexjrqm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kmsedrbv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bpwwmygb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jxpgdeqw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jytgyjeg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2evwyheyx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hftwpkij.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bwhxtbld.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2mbhdqlxi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kbrsqfja.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2savxmwbr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2szqguknu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ofykbcwd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ifrovqyn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dbtoxons.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yelfjclq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2arxfkokp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wawhzwng.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jcwavftq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dtorakxx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vibfpiie.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2clydwabl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tsmtpfuo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rrhwqgbw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2eodisage.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2tumpmxpu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rgfjucda.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2nclvwwnh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2heqxqoos.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2hlxiuqjc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ulzfowcb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2fasxzwwe.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2harxfbbm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gmaxspeo.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ncqugzfi.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2arnuznkn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vcntmove.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2etiiuipt.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2cpzyxdpu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2sjfpghcr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ozrkamfm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lgcywxjz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qktipcjx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mpzplgkb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2cpgxwdtn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wrlmemkv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2feakasov.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ghyknecq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2luiovvhk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2vgepxvtq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ctnrzcze.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vrzwopck.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vwuczyvj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dtgzdujs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ivvmnfne.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2lgvnpyhd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xpzrxahk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ttevlxbs.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ekdtrfsn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iobtnmjh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zfvdqpjk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ixqlyjxi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kvstmpei.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nmzbmmbp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cdafyise.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2veyochlx.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xjfunwqy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2flooibzp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2dfgcreeu.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nlkolevk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2kewgpdlf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2qbaxiegs.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zfzklcnm.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2wkrvnfgm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2xlwpimye.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2qcsezfrt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2byzlsled.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hafxxdjl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2btytibhq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jsineahu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2fychdocy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2xnimumhc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uslueede.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2hgwifkzi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2jiowdpbc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sjfyotom.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2vdskndkl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ltefmtnk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bagttsmz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2bfttlvgc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ksyuofoq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mrgtbono.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wfdwkmuq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2gbuvspip.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2iufwoadw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2fmjdrepg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gjwdwlis.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2texhuidc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wblhfqsw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2lcxzmyac.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cwicomun.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fzqcuool.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2hikububp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2dhdukqyr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xxnegcvi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wyefxyoh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ualaarur.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2acfbyijq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2uoholavp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2fogoqwyz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2iappuxwl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2izrvrzsb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2hexehhlb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kijfxdvk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bnmngwwq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2wfwkcltr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2daotrier.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xzvtrydc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2nsxcjxed.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2iuccozwk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2dsvurryc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2pfjxbyqi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kwpruqdz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bwudvxye.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vxgvrjbg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xyeazbbx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2nlmpuqpk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2guosfrsj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2mgzalzbc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2axncfban.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ulvogesk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2usirefqi.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2eujbzxpi.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2imgudsfh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2uaxtwnum.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2trhkvlsm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ekrvqril.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2untafacf.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2mibpsvce.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2jrijximh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2uuqhwnts.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2qcdzglij.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rntivpgb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2rttvgwiw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2eougymcl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2recjfaug.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2szlbcteh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2hwepcoke.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ddtfhfxv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jekmorxs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nhfbozhk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2aiwwiolr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2cifrmabz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2awxvijlv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mxhdwlxs.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2cumttnnv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhigvdpm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cbiwsjif.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zvkymvxd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yvrmrdgm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fvwlhgnd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2byiabrlh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mbiuiwvy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2alrzqtgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxwrckvk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2jqoitexj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qaxckbux.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cyzrwlrk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2sqosffip.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yhekokct.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ugxviatq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ffnjmzla.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hdakntwn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2bsnpgfrn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hzfwbmek.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wqfozobg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2uutkvaqc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jwcrlwqm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzgygxrf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwiluvau.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvjqnjlb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pupbduye.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2tqmqqemh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2jobahoul.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2knndqoot.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2pbusnlkv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gozkptaf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fpkqszmz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zkfnjpcu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2paxusglz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jfxqyzyh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2pwslqbre.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xzafyqba.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ybhjhztw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2pgxzdhba.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qucohgcn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2nijkmwmn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qacndzfg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jdtxmtmx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ilrrkvrb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tocviwfz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2efzpfiqy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2fwororpd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qqozrckt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ffejyuxc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2llreymzl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aqgmpswn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eptmspyw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vykpuztf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2pmukmzlr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vwcjewdx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lfzdnovr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ppecysss.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wagdawxt.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nsgnzxle.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tvdbtfaf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yaqjtftc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2riwivjyh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2inbcvych.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qbtwrcdn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2exnamyzo.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2glizyvmc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wqgakzue.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qicgdjmk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2tbsijtfz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jpqgwrim.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2cvznyoga.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gaimdvmi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mupzzeay.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2eyisarze.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2onuunrmu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mbhhqvqf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2aeusjdnz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sxqjfghd.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jbmgqdpx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ipvasxsu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2safshivu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ekjmljqa.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2pswcvlxm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2mfysrkcv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vmhhsevc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2idrsferd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rlzkumil.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2omyrffuu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ygjkvjbh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2qcixpnpo.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2peerhsqn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2dycamlwm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2drmnpxql.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vguzfyez.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mqvrttlk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nkbncxbz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zoshehke.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2pzdamjaz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gzbjskbh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cmezwgnv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zopovefr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2blrrlzen.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vmuclrjd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ilrhhlyl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2woapzkdf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2arsiluwe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rejmentd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2evbjfsqx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ubrqmhho.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2obwgdutq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2yhjgtzuy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rwhnmxoh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2gwppmamo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ffrobzqm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vhbmdnak.html


<!-- 参考信息 -->