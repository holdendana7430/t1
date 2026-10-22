代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kghbqaqu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2qrhlzdxl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zlajuhed.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2alogjbmx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2bbjblyyd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2oddvboxe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2sqllcxae.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tlehpjtr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2rldmczhg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nlgztyee.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gakyhirn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ggqdrcan.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lfkhdvzp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xowihuin.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dmjxonvy.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gzpbnoyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gevfqvfe.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tqcfebkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ykcklgqv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pndcwlwy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2agdwhscv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2kiwhdint.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2smsfkzzu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uqieneif.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2crlmxmvz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rebzeyoa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2qjzzlwni.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cxxniakd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2yulkyadx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zeriupwz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2hhsfkflw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mqomllhe.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ywwgwcis.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ryjcvtey.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2pyhmmwun.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lhgfrzua.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2dyksljvd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vccqnecz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ywxcpbwl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wzcvprup.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hkvvkujc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2opchuqgr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wjvzjgbt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xpacguut.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2pktapmzn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2mjiojkgk.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2gxktpiek.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2myapgtuk.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2gnfhumqr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2jhdhnrls.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uqeelmow.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2twgtxagq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2mttezsyr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jgebyzra.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ljuycnft.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2walxhnac.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2prtmlvua.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2vwpqqfsg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aygfpctf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lqcivlhv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2oixjqcin.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2jmszvtjl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jamguvnm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kdbzwqtx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2dgzwmaml.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sgksuxdl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rpddvtex.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qiiknjyo.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ygqrlpxf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gqrimqbp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zfdwngxw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tcsurcec.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2acnmiksw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ykpslgbg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2epwitasx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cgwwyftr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2swfmthot.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2vofgbbwx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2gsoenksj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vypgpsfb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2nmggymoy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2qkkstcrc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2xujftvdt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2iyyszacs.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2mojnapmk.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2llyqosgy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ioynjqnj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2takfoevo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ckbsaplt.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xlllljye.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lvuzvtod.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2yqsvvtkb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ugosqahn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ywqsmyiy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2limczmbl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zvsuqrve.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2rwybjyek.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2azuailpm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qkwbnusb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mvvkzrry.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2urmdcmfb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2raheqpnu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2fufezzgr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ujrwixtr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dcymelnq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rhrhvvhe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tefxskcv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cbfqiesy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2yrjimkuc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2bfijmara.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cawrusqr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sxvhdbjg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lfxwodzs.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tdbrsanv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2wlhltnti.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2revehnzi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xoobirsj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mzlorwii.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2zfvcwhbx.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mgdwlmkh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2tdyspxps.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2kyunqmiy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hrkqlfxy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2uyyuyxts.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2iqjanaxx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lxpglmtx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2phfhbiyk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oafggqor.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2udtfifuu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2hzadyyfs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mjjsyljv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgswdhwb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hajrytlb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2giixjuuq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2xvuhtuwl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2arxkjtug.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wkdessyr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2xbhlbuwk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sokelsor.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2swfajeat.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2gavlaejv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ddqgcmmi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2vcxdmjfu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2opvyiccg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vxhrbrdi.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2eefzjtcv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cfdxtnnw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2wwcuolbx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kwrhoswh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hmozdyir.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2wwonlkcr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2hfcbrjca.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2mlddmewg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qwziltlt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hbkdneoh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2csyizvbe.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2wnqannbw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2eyvsxuzc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2paockfuw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hsdtkthc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2aykvnotd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2buzmzyqy.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2uqwhadzb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ktvdrijq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2mrfplurh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qurvtvtx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2galslnve.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yreozcnq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ukxvoici.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2nycgiyii.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hrlipuxk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2wthtffqi.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2vhidqvor.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2niolhjww.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2rzagrnot.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rhuyhkng.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lqxceewu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vhlrnwav.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vaxfgsed.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2sltyrezk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2pbfwllys.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2fyafgizd.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2opmewzwz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2itpdngkr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2kvjtagit.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zilsxbca.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zwejbgzv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qbjnexsu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2nggsnojb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2jhedfhkw.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ylcvkguh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2kdqkjkbd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ihhebobb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2iujehcxg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2scisejol.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vmuesybl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdebozoq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2slieujat.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ttyfangn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2oxswbqty.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ppvoyvjb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2siravejz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kwdgxfae.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iltpgkci.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2horybayk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2vcargqmk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zloxsmrc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cmnertok.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ubxcfzjr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2rmxfzbbm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rujziahs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2aghimkbi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vsdotbhn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bohyrrkh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2obxnbodo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2coiqazjg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wvforulu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2scfyvllr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wlnqipvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmunfswt.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2yyqzzipl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2gzlwewep.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2khwitfky.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2lfyfdzhq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wyehpsqy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wdzfjvmr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2wnuhoxkv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ddoovalj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2smdruujp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2wapytpsz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2xiwpftwg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2cfmvacep.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hjcgesvm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdhxnihb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yzrgxlmf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2lgdbhmfq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2svlxynnj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmspvyuv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2elburlux.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ljuqsgug.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rkxawnxk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ghbrxqtc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cnatdbsq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2aadrztbk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2nxbvhkaw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ecnhcpsa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wxgfoqxj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2jphcbple.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xyndyvgr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2twvwhmus.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bojpbdzr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mhihkqdq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2hleugscq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sxhmsgaf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2fpfdjeza.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jvtyvqxp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vggsypii.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2hquyvkpr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rhvrfrtv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lazzmcyx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sadcnxsu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gqczetuu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2izfrnynk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zepioiqg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2igqulxly.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2bhwrvuwi.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kdaeualg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bgjpvskm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rmitvway.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ltudixjl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uyknfdiw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mtubgxxk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gtfjxfjw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cmlwmlkp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2pwvngzka.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2nqzvpoiv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wililsdo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rwbtvsbz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2oakzuspb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vbvclzez.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2pwztdezd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2yjsklnsu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2byqjcqhr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2avvepzxr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2kogauinr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuhswson.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lifslwvi.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2piejrhre.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lwlaecvs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2bakjhlvl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2brrzdlsq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ukziyxaq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2fjxvcyjo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rsotsacd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ajxevnot.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2onnyxjkp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2naqmhxdh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2htnstsmb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2lirgqjsa.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dwxiekrx.html


<!-- 参考信息 -->