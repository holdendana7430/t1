代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yubjhtwp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2tlnsbeco.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hymxbujx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2msmqccun.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mjppkkac.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2xcasjwik.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2oayvpojo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2rpmplloa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2fbhqgikz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2wfflctoq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rjrvpzto.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kkkdrbna.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ddgfvqzs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ecmdjnjg.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gyrxgvfa.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2sheacfnt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2eypaefuq.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2mnsaqlxn.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jrriyetn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2stedwiyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bukgjycv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2xvbyyoox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hcyrmmcr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2midzfoto.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2fstexlmq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2cvxeuddo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nulayahi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qmrrfkvg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2zlkhbxet.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ipwmltjd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2iaurtgzu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ziregbak.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2zafltlnp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wcdkwihh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xsypnnps.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ixgqilvj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2byayfzjy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ddyoyozk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2zmctvcrr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zgvvbmxa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2euhvfyos.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jmvtpuvr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2zwfdunhu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vevkvwhg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yoqogdee.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kqorjugw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hpmutfdd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pcuajxrp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2fxwilusv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nfaqqxld.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2yrfabwwc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ufrxkboh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2rwmaszsc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2zbcbhvjc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ynpbpykw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2oyzvsgum.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2eiqhkwmz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xyjrbdsl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ututuljk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2tuzckuam.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cnwnumro.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jezlkslo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zfblqhwi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nrebqmeu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nmeysenx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2yxrintdd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2mrqrvose.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yowleupv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2wfdssqrb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uyoeirhv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dtbfvlpu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jrulvyej.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2imhtitsi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gtcrwltm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xsywkzrv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yukxajnu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zfasqnrp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lzoegbca.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2tyopwimk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ncntdpdz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2yxuhktbb.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tgcfhace.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2myhymddp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hjvxfxtl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2cqdwradk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2zvuwgomj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2umshrqct.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2quutqegl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2najrrsev.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vpiciwxw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bbzwekjk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xvxyezta.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2vhswlmhe.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zypyawyo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ykoggvzr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2umshexph.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2fprkpxjk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xyanxalw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2miofgbvm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rosjccol.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2fqsgvptr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2rorvtooo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2coyvuhqu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mxikjfpl.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2vmaappyg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vqyicsml.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2racgphqo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ztcfiwsr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2eckhuewc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cgmbwuwe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2urzhvyhr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jirblugh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2bcautrsk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wkwdqagu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ydzvnlyy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lkniarti.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dpbxehpr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2biqnfpkh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2eaertpei.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2erwlmtem.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2edzsiaxr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2scsuugxx.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2qkohlknx.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2crfykiaa.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2zovyvbed.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zaxbuqwm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2uvizuajp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2cwdsiogw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2dfgivlqn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rbwyicsi.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2tpqdnfpn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jvpwtiti.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2kzgpjlbb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdpdbayu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ceaunlzu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ooasfdwt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sitdiyzs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2stqfgxqy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2pgotloku.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pjqzdnkm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2draumpge.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2jmvstnoi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2hahmlfxe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2soxmwinm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2avjlxddt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vxkvyydw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2tweikbrh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2cwfmqyyh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lajnnwsv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2scevklti.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cabrkkts.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nzdwtzuo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uadxfotl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bthirzhk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2eztdscrt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xakzjxnh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2drqsmyjh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jirzoujx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vyzggrdu.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ceebjzvq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2etrdkjtz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2yovgzikr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2skgqbywb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2aipirocg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2jvgtqjpb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2oikctibh.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2msxkbbwt.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2jjpqtona.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2uadkzitf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hqqjynzp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wejeeixo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ukjtdjcr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cppyaswp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wbdmqsui.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qkujqffe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2majtmgdb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2tnfuwqxi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2nrysqgnx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2jlcmlatw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dbsjomuh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2euvoouvo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tyzpavcb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nsegffcs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2xcmmcwnf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fgwcsjef.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2enuprfjn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2fhzgcmbp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2timpithx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qipbtzse.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lwqfvtkt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2jwiswdqr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ewlbusiy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2zivzwswa.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2bdelukkm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2aksnyeag.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2kzatpsln.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2evgusurp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2xrfcayrg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2zfemtjhc.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qzmalkvi.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2vpgbxgcb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2xyjskmlr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2oimikmsz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2lkjruayx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2tlpecytf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bayfwozh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iiyedfmu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yigegzhf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qekrebvc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2tbzauisy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2offslmqo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jyeunbtd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ijaioaaa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mtpvhozr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zbyutovw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zmbplhqm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pjexqwza.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2oaozaadn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2bswgxgvf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qyogtlhi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jxvklnzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oafaubkc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2txekvrjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfcmitzh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2iuiccbrf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2gcecdkgg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jihtydgl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2agpdllic.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2soelqwzp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cbspnoqh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2plbdtgvm.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bdylkqso.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2djduxsyz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2goiizysz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2gpjjzdxb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmfkjiwu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jlgszbho.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lmmcyzob.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fmzirapz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2fdffjmvd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2fuzkbelt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2gfdzppzd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2tgddbxqu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2crfxumlx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ppupnkvq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2evgbksmz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nnemlcpg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2dpgfufsa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2kxmmqhak.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2slfhlzpb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qvjgpiea.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2yzmhmhef.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ktuuxzqo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ueikfhgv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rqeybeet.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qqwdywzf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2rhekhzqi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xttjqbmf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2jxkyacjs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wivrcony.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jpzwtqix.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2hutursil.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uqythptp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mgzxgeqa.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2syuztwhc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2puioxuvv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2yohzqktb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2suzlqcts.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zbjohjft.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zaxhvphv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zszyzcin.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ilwefqjc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vhrfchkl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yvzxsamw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rdlpekrt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xezdgych.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ntoypzac.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2czqjcfmm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2vsoibgdq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2csubhizz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ocouxcur.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yevdmgod.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xzoxuuct.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2rhwnvjvj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2dnxuricc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2sodrkrxf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2lyytcuel.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2leqpiwsc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2lfwahmea.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2cptknqig.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sfnbdnse.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2swahxlfw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uwthgllq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2almwrukg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2fiferldg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2wyzdutfl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2rncjwhbv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqaldltn.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bazxmrly.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tkhewvms.html


<!-- 参考信息 -->