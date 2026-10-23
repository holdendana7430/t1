代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3dwukbuyy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3lqqpybkz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zjlnqyrn.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3euqxgtsa.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3qtlwqbeh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3gbzlqjjl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nptpigkt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uoupwoax.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3klhwflrg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3rfeljctf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lqbygtnt.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3lqadfake.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqpniwqe.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3souwleje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqhwwtbe.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3whwmwzku.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3frlvfskf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3stljifgd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3unjojziv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jqlljlbw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3sgugljpy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3okcxalvb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xizydcpt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pzxozvkp.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mrqfoekk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bswukewv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3nxzpmpfj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wgralbxf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sjwlsibk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3raffxxdt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nhijisjt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lszkzsqw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3kriazsaa.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bkustlip.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3fhcpqwqn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3holzmdbo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zgpjcmya.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vksxcjly.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xuwyyrpj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gstgodtr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ytgblfow.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ekerpxql.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3xdzqdlvc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3dxnderdc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3euiibkmb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3slueijmr.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ujlfajug.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qnjppplp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3akrtevfw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gpywcbat.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3crvstgwz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3yvudpnyy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wztpdnxy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3oobkhkmg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hohcfold.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hllmlcji.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3azqjqzhm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xztzqclb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xpdruhvu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xwtxidyh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3agobvomi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nswbdnta.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3njuanblz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yeettmgl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jkhhdjzs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uviwdeii.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3oxotgnbl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jxictbqe.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qlifqndl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jnvxfzvn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3tzolxiak.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xzznnzak.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3andtvnda.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lfcwrwom.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3bbuisomd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yyzwmtjb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3txhnnztm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ifvqahij.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3gdzysial.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3qyqvbsxo.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3vlebfsbk.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yvkfgbun.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cryupyjo.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ckdrzbqu.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3dsffxyul.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ixvdlqnp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hdsicarh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3wykmtbkl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3qzmtdifb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3akqwejzr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3genzvnwy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bkylntep.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3trwqdtsm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3dhvmfljk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cxsdlgjx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jhcemfio.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3yrjtmatq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lqrjzqqd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3hrxbbtnv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3srufsxbr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qgsbtumy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3flrlhjcm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3peuqjkmv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kjlsdyrw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ofudvbtx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3gnbfolrs.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pqwwqywl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xejrjodw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3alcnivat.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3twnreyvh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hzbyiygq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ogqjagqn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lvcbckkm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3frnwyrid.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ecqdxauv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nthkimrc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3qemjbavt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ozjnzxye.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jypedxqf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3urysmczl.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ycxnoxvy.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tgguvhbi.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3grufjbpc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mbofbfit.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3fisgpfxs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3dmdujraa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xhbwkvqn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwwsudts.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ineukpcw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nvwmtxdi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3jzzecvuy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hbtlodzb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3trreycak.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3vgdtmybw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3thsbyelu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3oiuzyqvp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3gzkxnydv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3myyzynhz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3rzkqelef.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3pqjimkgi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pzbbskuk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ibufipvy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wjkgpwyw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3yrpeyxfe.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3viorqgkc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gcqkdbev.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3abwqewpd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3bzmeasoe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kacscuox.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sfmjiudd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fmmuaizf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rhlaguxt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3kvpmejyt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rxiimrel.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bsjnfyve.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gvycxhrg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3vtquewbc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ownbeejv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3znmlalqo.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3nkounsfe.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ndhslalk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ctsifqis.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nurybfdf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fuzruleb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3dyxcbjle.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3frkauwts.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3phhvftnz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3uqjnborn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3laksakqu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3kgovpbjt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3iaptltaw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nvvbppfw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kuzvkblw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gcwqxwjq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oermepgt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jfqhanpg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3eoxkzivz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3owtcnvdr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3rfwnsfeq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dfbiwzwp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xunolbzs.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3uttgqpou.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pbyututs.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dqvszdku.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3tgsyoixy.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3dnuvggmw.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3mianpgip.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3gjoecdkv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3nwnqfmyt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmqalils.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3xocspakm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wlpqfitj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3crmxlirn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ehodgclo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljphtkbo.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3drfcjmpr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jbcvaikx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3scphyiet.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3efgbgwki.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rqpbzxwc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xbrcnbkc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3pakncuyz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3amrplwxs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kpaaehuj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3vbqxvzcg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3bgzkpqdu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wtccvhxw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tpizjwmy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3enpbbizl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jqoxmziu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3lqfxgydj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3evfkgvxk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kgqfrnec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kawfdgyo.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3rvockcbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xydsjbea.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3yvizmmvs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3iceznqfx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gmkryhze.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3wpqsfxdb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zesitxsj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iriitipg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3mtrckojf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dohzgagj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rqgrgerw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3aqtrjnqh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3rhrnyhqz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3nqnrettp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uayhvzth.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pzsrwqop.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lbbdvewd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3voeummju.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ezlnacef.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3thvmvxkx.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ncdexnww.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hwedigkp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jtmomjfa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ghpjcrsp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hlrnnvmu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wyrdzbsd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3btilnxrb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ukmquwod.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zrnwjyyq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3jawbiooh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mllsopso.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3bvixotrs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mlrcapgb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jguvmpto.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ncfjtdzq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ktsdxkuf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ilftxytl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3xtqzhkoy.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3agwfkjyj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3mcyzkkrn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ovaatira.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rdayamfg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mxgfmcfa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qwygfhyi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3xlsigfpk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mlmryywc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rrwhirna.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3zadjbvjk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ntrpcgap.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tgocrgid.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xgchudro.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3grskzfay.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fzokmsil.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wliojwlg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yplsrruy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ltjtecgr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3bjayqfvl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rlxpdiun.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ubudniph.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qflinlqb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3joecxogs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3kmvmgqvi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ifbxhwek.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3rvdzvbfr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ehjvjvtb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3indlquqk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bjhcykdj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3crwlcqsx.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3dphirnos.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3juefqlsy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ctsfjupx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3uhyrtwki.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wgspajhr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3eujtzddp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ztpzvxia.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rydzrcrf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dwkhecbb.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3aumnpgms.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3eppjdmlc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mmkzyovm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3jjhmngio.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3puoivgeo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3mbvyfdnz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3wzgwilqz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tyqweqvj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yxnmqcpp.html


<!-- 参考信息 -->