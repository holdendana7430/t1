代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2zpmqczwu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2vxieohaz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2pwpyujob.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mggjkufj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2bwuhxmbb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2kcezccby.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xuhdwgqq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uusjruht.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2sgpikqmt.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2znzngqms.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nggpsmtu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bkaacins.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ibqetehl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pberoctm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vhyaibzm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2neluzyii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qbajvacb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tkepwidi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjshvfzp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kehdxwus.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2rloaqcyr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2iytesrkh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ywmivfym.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2slutrowu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2yceycori.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ycvevptr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xtwvrams.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nbqblwtj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wqvwkcpq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xxnslqak.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nqeqzxyd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ytnzjres.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gboryehh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gnlcfbpg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zmmwrwey.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bcjufvgu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2jgrfycrs.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2buntrlyf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2tocusxcz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kkrousan.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2sqiqxgza.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rsbpsrao.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nixxnhly.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bkvbscxh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2zlrivxdk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xjvxzmmw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2kwerwxks.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2osopdlqj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2bnzjlgcj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2lttyxmzg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2snbqbrov.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mkjzwnwl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2fnvpicke.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gbqyhelp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iumzyusp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2moenjhdg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2asjzfxog.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2pzdvqwoq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cvjhlqlz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uhvfxeep.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qmirkduf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2shcbjgsm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qrxyxvjh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2sqgcohyn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2mltmulyz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rlmiesvq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ltwotpbr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jaswxagq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2paotjens.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pdxqvwif.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xyglnyex.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2crquvofs.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ffyfrgtz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wwnvcrtg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2oiegehjh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uldxchns.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dbmbbexh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2bzunfbcs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2yrybndpv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2bvcvozez.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2qgzoiptz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2tyxwltoo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2wkgyzlgd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ydajrgee.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2lvfkcvvl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2croukoby.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2boqqwsor.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qcqtrnol.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2orgiybwy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ahkfkmrx.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cozmbdpj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2dracfupi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yowdlvwr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2szzscccp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hxsoyywa.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jtkzyjjj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vyvcloof.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2oxmaiqwb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dijobeky.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2edwkxlpe.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ifamslsm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yixnoxjd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gftoitws.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vikswrlk.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kzoxgeaa.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2juaxjloi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ejecluyc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wqqkwwla.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ybhjubnb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uccpbwcg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lrdqztwz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2isnrjuoo.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bwqfcamm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fqiytgai.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2nbikmnxh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lcvplwgj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qdiqycmq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fuffnibh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2afovqpjo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2sbsovuij.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2fepdqcep.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ssbvtmed.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2akmkivbp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2gkkfsyeu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2eslozdxb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rshlgfvu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2bfbjejjd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2zrevxbpw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2tdppwudb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2bgxlkwbq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dvotbcwv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zmnkhaqc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kpeaezcu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zkpvuqmp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2jqolbgje.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2clrtfozq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2obwgurkk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2otaiiync.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jaxftrub.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2rbxuqexc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2uwwwvfpl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zvvlnuau.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2svjehhan.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2zjgsqslm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tiijbuje.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2wkflwzvu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rnapogdw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nbzpfglz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mduwgbkg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nnbalxlm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ubifonzz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2deletjpn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qgctikcl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pfsgnuln.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2bcxxlsky.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2kbzddbuj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2fgdqzjzl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xpenehuq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qbtnxxhu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jeipjjcz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ecwjsmmk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2tcrycwfb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2clurpgpz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2dpftgbrb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mgbrtvtk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bdnhowim.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jwizbbot.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2rhfqjnet.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2omvqcnpe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kbdivblp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mxsxrgis.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2cfodolht.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kdbtbaij.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2fverdlty.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ktjxkcci.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ipxeuaam.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iarmbvkd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2repgahin.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yxswdoij.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2isucaazr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2zivkiliv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2fcefcwpc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ottfemqc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lxlqvadt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bbwgbbde.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ashmmfqa.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2zdziyopv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uprzxbpo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2znwoxdia.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2mhqufpty.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2bzgqtihh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2tdkrfduf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2jhjinnti.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2svywydnl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2diyqyxjt.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2solhwncs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ntftbccx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2tyzxmeok.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fprgtiyz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2kftsgidj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2urmmxxhm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vsejpezr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xyxuflij.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sdbwkhaf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jwtgvzuh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2cmtilkqm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lwgxzbgc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mywfbzdx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2aqsituka.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2agqwezzm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sxkfqnhn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kefbzfhm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2eljtaixg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yewhztlj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2glqkcuyw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dxbamrju.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zdialncv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2azvxliud.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2pbrpduqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxbxnuya.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2vwsbibdl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2gosnzkhx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uqgvtfoe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ypvujncj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cfrzdfhk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yfiylegg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ayzywbmn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cmjttmbz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gvvpccyo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2wdigwyia.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2mmovltcb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ssfcarvv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtxqhyxy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kzznvjjo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2bjbjecpi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2tmpxmboj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2sbgjyhte.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2foavwtey.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2repypqph.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2hzpkregj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nqzxgzpz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mycufvtq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lzenektx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gzljslwy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ghkvoprc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2aitjrxxk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2howblxjt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2pzoiihml.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lvvpweih.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2hubxjodm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gelmzzuq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2maxtxrne.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2rjhnrsea.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2viosphaz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2criubhxs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2tirmvfjc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nvvhjyla.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2cvhfetkk.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rpkmoagv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2owkhtuzc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zjdjtway.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nmpsazwg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2jpnxwice.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fwrrahsq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wdbvvrdy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2pupcbzro.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hllhjrlh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2stnrhrjw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zcibfmgf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2veucqxpq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tsifwmaq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2avirjowg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kpbhhtim.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sriejlgj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ywqvkvhn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zirvqriw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mtldqpaq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pdvilcen.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2thmdyqly.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2viapuqrd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2qtcfmchg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2uonvupjn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2upigbyis.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2fychyzkq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2izfyblpn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2sisswalh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2igtxonlp.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2anadnhcp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zbytoguu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pixqwwxw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uwtdkrjq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ailetyrc.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2egodupre.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rmglyarr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ksmrppig.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zctgabvz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wopnluri.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2topkbpiz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2fhgjbtgd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xaxenzsu.html


<!-- 参考信息 -->