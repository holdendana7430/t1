代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2shajwxek.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zselkgxb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2huaqandz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2iwchjdhd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gnbtsajv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2xbsspavs.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2lgqqwwue.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2amnhlpph.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2tzkdsxwo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hunjpwnz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2cqpqscqf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mhltvniq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2erjoikui.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ixiebjvi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qqifycwy.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dovnxkwu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ghgjflcq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2glexaqgf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bublklsr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ttovvtxx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zydwupao.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tyuzdbuq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dfamguzy.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cssrjmin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jetzubfh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2haqtwmau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvqirbus.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gsywujvh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2fgeqfwjg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2kzcnnyhq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ccrpgzkx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kxwtrrer.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2tzwirjjb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qtabpoxn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2cxtmjmtf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yglwkpef.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2gpgfvnym.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zsenzcso.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ajymwsip.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mshhkeaw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lkxwftme.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xwtoidek.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ylxafibm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ouazsrzq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2fnrqujbk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fcecqpua.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2uneczktq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ciydajxd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2svlyygci.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fyrynycs.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jbnnigwh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hztoiwnn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2imvhoofc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ggpjrqfm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2fbfiwwjx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rhzhgajq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2dicmqkja.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2tfcxsjnu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2glmbmbsl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2irmlrwhs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ntciatcz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zibptryh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2frezthcm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2rrdargbz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jymqaovb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2wcxpopjv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jlfbetrs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wgfnunrm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fltpgvhz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2wfizpjez.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rivwwyqa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wsgdizss.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2exhsmxft.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ajklmvzj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2rhgdxecv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wnardcdz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dyyyokqb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kgroooki.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ytkkmgxe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gdgwtnnr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ppclrqjb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2lhsgdqnr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2vxbsjrbu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2grlxqcqp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2idutwkka.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ufqlpamw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2zglfqhji.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pekdrhmc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2rayehkuf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2katoosxi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2bgwtscqs.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ovpnrufe.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2qekarpjl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gdwncqqg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gbefacxx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2woduedjp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2fqtiiwta.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qnhmecul.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uiamueek.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ttzcmubw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kudsyvgb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2gkameqpi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ljytmupd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yuzcufuo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2pfewlhbc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2eszjigvq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2hixbvdtz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2pzbyupew.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2nsjjtgej.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xqscmzge.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hwtwbbxp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gtgglrsx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ivobyljj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2aveqczdm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nycbhfrc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dnnfanph.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2rumqpcse.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2iehrubip.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wkclluvx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zkombhph.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ojkcnpop.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ajhlvniq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2okccylbj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cuccznva.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tasbontf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gayylobw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2leotlcnf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zjrljlbr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2larnnfcf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xadihunh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ycxetxmx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2xokabeud.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2qslypcms.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jdwpvgmy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2gfqbtxtb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2charkpia.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2utsunkmv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcheixut.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgxmsuck.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gwljuadu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tgxejipz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ybwjnvst.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ebcwpxup.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2johxkrwm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2brlkvfzb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ajpehbuh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aurhgqnz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2daefszhh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ybfxyhqb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bmyuylif.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2kvdefeqt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2oqswgvyb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dcepqpio.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2tacosotq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ifovrhxy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uzspidka.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2vnkgkzdh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2omfyidgx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2mqfyjxmi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2hbnsfddz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xwhlyktd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qevuotbd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2qzzkzinv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wbkaxytv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2kfxseeoq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tthivedn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jjpiaigh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zxxrgwqo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2lwdavezv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pejsebfy.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ongkimjf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2jrzqacag.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2umtasrme.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nwkvctim.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2maqamxpj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2tieudefu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2duclgwjf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xnmxmdcr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qthqmtpv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2yxximozk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2mzlbfqrx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2wrswxlhb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2hqojtmul.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2myrnfuho.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jldpbffi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2eoaisvcj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ifmouvea.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2twhxwnmm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2hfpywkup.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2atjnctup.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2alyrlkfp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qryieibf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zkqrsnpk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ojfhmhih.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2totibqfa.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xaytzbgx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vfnatvvm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2uvqzkvdq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2cdsqciqu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2pbbpztdj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2dhdyewep.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwyrljis.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2lvkuxigh.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pftlhwuq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2szsrtslt.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ondnmgjl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2qrsydhsw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2boapyfjg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2dcgkrglc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ayzrtzvc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dumwsusi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2datpvnhf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kgfkrdzk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2obbpxtaa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zpqxdnxw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wunslywo.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2hmvykoun.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2iymurcsc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rwlibstc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ggorkeee.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dggjkupo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2klmtcvtq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2cxpiklfi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ymtjsqib.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qeirrgep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nytktylj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2nqpwmpmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmvxbifq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xlaajzez.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2kvkalppb.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oumrtysl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2tbanotrp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jphpplxv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bexuabbl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2lyrstyds.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gorgwkkj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vdlobywz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2rjfroujs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2einxgdyl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ltxqqrrh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqchmbfz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ldavzsex.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cvgoellt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2cqzszuip.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2tmxfvlgx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjtgffox.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2aptifbdx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2zecgetcs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2plnfclnl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ryizofqs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tvmuntud.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jgxqprmb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tmocffud.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zoazutvd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2iqjvcyyq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2tyaaikws.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ntqroiut.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2fmiqrish.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lrrpxask.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ivalexba.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jrphtjzf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2msnlzrou.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2rehglkgt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2auxisjrc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dfsgqufy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2wlaheqjq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mcqbfvxn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2whjsgeej.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2htlfaxzp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ercytceu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2fztyzqay.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2klydjvyy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojhzcunu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ejxvmrju.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vtrcvebt.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dcmithdx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2knptpbep.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uogdxycq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ioonhacx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qhxwjzzc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oouyprjw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2btxgcnyn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2gwibafaj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2effzvutb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jjnlffry.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2drbuibax.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yudtxaba.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2grcxyqme.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2dgsrjrfy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ylhqzasw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2bqghdbzx.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2sldevnrf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rwsqzykw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2xexamsht.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zrzpesss.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cidtcwre.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pdmzzpys.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lchouiht.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mgfamncb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jxkufhci.html


<!-- 参考信息 -->