代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ibczaljt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3zffnhlaf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3nqhanwkv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3qestcvss.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tsrnjswi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3gzmhasri.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3kmprhuqg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3blpaisat.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3vgpgbpef.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zceqodzh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cvrnyijj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nmthjcgb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3mkcyysrf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ukjqxpaj.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gvtddqqm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sasikltv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3puicfekg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3lsetednv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hyyqnmza.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3eddlroqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3belbzfdc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3zbnlnjsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3apzdbmpp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tagcfoqd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3waylcqag.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3rzpttxbo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dnhrzlwe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3srzdlpvl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3iprngdpb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ddzlayhd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3asqcsnmz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xaemapdg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rgypzrqh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nouoakws.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kgyqgwfl.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oystdfzg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iciqjzoe.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zuachtaj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kgcoqzhu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3eyisuhfm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3xpuvvnci.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3leqqnxfh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3cyztsfwb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dnqmwsvc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ahqjipaw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vzcpoamt.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rlhnvrqp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hkieqpye.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3glcdrsut.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tsicespc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3bmfnhatc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lwhvedgc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3pbpgxhgz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3atosyakm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tutsjjnv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rmrkhhgo.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3rkpqkync.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3upcnwokj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bvgkisir.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3jxhufyju.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3abykmbun.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3sqownlnx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fsvyayji.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3blylsccy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gcdzegst.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3kutoxdnp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qmmakzqb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3epgqgwhu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3kdwapsyw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gczvgyen.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nqridzaq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zssbwgww.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3orqccmkz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3txamypbv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jcyvigvh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bjfnxcus.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ngfujvle.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dckfzgky.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3mhwpmtzq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3balrqktd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3rzzrwbai.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ejhxevat.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3yliiunuz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yvlulzfz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3xdahklhv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vxvaqhqw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ydahckzd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3nmewnhti.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3yrgyutrl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cfgqsxhj.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vgmxglug.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rhfanylh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3cyuetijj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3puvyxgqp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qyphwaej.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3opsruwmu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zdyhvfdo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3exnjoexl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wdafcpus.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gwwxaspe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lzgnohmy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3nblyxgln.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zuprpmrx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kbaxnyhk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3moznseky.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ijzlqwfm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3llpyqipm.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3iadffbca.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vqbwcsyc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hjkhafnz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3guelfwzu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3blhaczah.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3srnwiuhs.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3srlbsice.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3phdgcgxx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pzxbdiss.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zrwpgicu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qyyuvotc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qkrkzxxu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kwowiiaq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mdsojpsy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3gytooeno.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3iqsoqhbj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lpfopbld.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3tvsrrqjb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rwvotzqw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3iklpqrla.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3qinanlxg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ujlifhoz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bdsmxyhe.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3xbfwvgro.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3asoryzds.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3jnlhfikb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwjgpomh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mspqsimn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hsjsbhdh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3isbldbce.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ogmbttut.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3bdrjkxhy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nssckqoi.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3sbyrpncy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3xvoyhxgu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wfsfvjti.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3lqeeaglr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kxysaufb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ydsgspdz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3gwkyemii.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3qfuhhvuq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tfuqtyjn.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3yywojxrq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ebvidnxs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3xomtfjwz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sdacewzp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qzezkpou.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ceyoirqy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ximgbyxa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3fchldwxr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nmofxwwg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3sauadmiu.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rihdxnzp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ncuffvvw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fangpmbd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3sszchgkk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ivpizdsp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3jeuqhjgx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3swijsdxs.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3hzsfvqnu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wurfmvpz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3cfcpcipn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3rxxfualq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zoyxvtvj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tqgluqmw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qgascvdt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3zgtalclk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3bcfizrpm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xceyaaxo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3wxzjhqmo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3mymvujhi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3gqblouzt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3empwlozo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ttkcdzrm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3obsuyfzt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pdbmcqqa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3lggegrpa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3pqsedtte.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3xawpwmlb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3lhwvtypq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ogvxniqo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3napsgaqj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hdvavzbv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ekanvsjq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mbnimwxs.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3vgdzzzwm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3dzikgruu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3aalwpipy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3wsiogcha.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3clubfjmq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkjwqmoa.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3yabvibmn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3azofqpqp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3smohubtb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3jbiufxlc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3fcipsqxi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3xdphbonf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3djnurifz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dgxfpbhb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ulkjfyic.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fiagirfv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pzjlvhvt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3vxiijepq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3arjjfkiv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zivugbwk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3juxisxoj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lcljgavk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yfyvquag.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ulzphqiy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sptcjful.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xcktofkk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3yavwsjsf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3szlubgtd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ovepeuya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3txzciedp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3tqizhitd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3liklkhrs.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3zdwluvjb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3twcjhdyw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cuhidvkw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3djaqfkyz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mghcpjdp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3skwwjzdm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3eloaiiny.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3roesvyow.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uoamsamv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3exhquqog.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3cyllnigh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3yztwngtk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qovjmdww.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvglggtk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hfgznadt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3fbztrmmh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3mivhkopn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxsahevr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3tcexjsxy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3invhityt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3letiwmfw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wrqperxl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kdaarxap.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3rqmygrnh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fwibabod.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3enrbpzkk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ofahlpmh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ojabqjfo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cemobekc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ljbuzphm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xsoowvnn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tehekrcx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3nzredezm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ajgyxbtd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3nuulzjbs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ehfdvvwo.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3octgzwvq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3aplexfxn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fzotdowu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bylxriyh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xevecaba.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xliykilb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3smlqwbsy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3graumhzb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sfcxdnof.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3glnedcip.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ftaklipl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pwpwmoej.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3slmjussh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3usgcwzvb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pyotoder.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oaagqclk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mroefkme.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3emxhiltn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3fhuasvaj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gydruelc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ojhdtltl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dzetfgms.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qxgdhwfi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ktaaaaxz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3gbmjiycb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jmdwfwae.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3qdxopxyy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3cypqqhdq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3scokhirh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3uhqubsbu.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3dpeiwixh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ppidxkey.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3gapfxiul.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3reyllmfo.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ixgkvpzt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ktnkjfii.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3cscrbzre.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ahbjjjex.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oagsvjlg.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lhefvdze.html


<!-- 参考信息 -->