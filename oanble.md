代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2higlurky.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2lpovzjzn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2savnzqax.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nlrwpbkx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qwquyxro.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2okzyygzo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2sipifemo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ffgorkzn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ugfbaqqr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2vzboiyvg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ssevfqgm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ehfnmomd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2wmscrzji.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kzlqrqiq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2sewcmcnz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ceybsvdk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2tefvqeol.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2dsxbsrts.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bidkrzal.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2grzwpprj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bvjmaasq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2edphpsjp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rvuujgew.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gahdqhlq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mkjdxmiq.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2fhptkngi.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ssepztgr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bbjrdzyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvoenmfp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2lphkvifb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnafmamp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ynmfclva.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2xnzfeuau.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ywzqswek.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2unnqfjbl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ybuscuhc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2thsaruiv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2jewqyoie.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2vmsqwgmc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2itvjejtc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kgzscjbt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2yykmsitt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2xnmodbpe.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zeuwgiba.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mudwtmiv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hjxigxxz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2xbuyyyay.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2kutpicnx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hofufhxz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gktetuxg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2benabuui.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fmieybat.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gvgzykso.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2falcdjzo.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qnxgeoeh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rulzsvbe.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2yslixsoo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rtbhrdbf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2gozenjhr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nfuaexcp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2oqupepyp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2gekrlduj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tfspawgn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tpdsjvfc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2nlviagwl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dalvtjqn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lgobzekh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2uxkwcvqy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2rhkafhvz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2tzxycmpv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2emuhemkf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2psyenlvd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uciqnqbb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2htwazpyk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2bnxrvhxv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oipypvpi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jjieeuvr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wjjljliz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2redomrqp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2urxumkwj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eayoikzh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2apzmsxnw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oibrhuqj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cvuqyjnj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eveagplz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2aylidjpc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2jiybhnqz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uyvbnygz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2bntgzowx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2drtyooxb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2pgxrpgse.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ozgojimc.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wznejkzs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qehqbson.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2righuhwf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2nberunsa.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2xuwiytwe.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dbxdofah.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ktdbwvop.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qmtofzop.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ibbensky.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ywbcdmqe.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2uxfwenej.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2jjugddqe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yfawwqlw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2vmympxlh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2umlbdudw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mthijqyb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wrqpcwpa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2puunxjiw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nnnotfpk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kicwksik.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2uibaaggt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vmxamcoz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2oryvvahp.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2coiwvckn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bcaxiley.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2efryvizy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2oszdmhmz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ivpclgcz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2mgaxfbml.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2djbomxyp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tmoebxzv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2thqlulra.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yppputor.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2svnlfvwz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ozahpyxi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ewhmgcxg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oeujpbze.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gntrspxo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2mkhzjhxi.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2oqzfaqmb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2aqqiwdmw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jxtwncke.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2uxbqyzok.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2jewlxmtk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2barvunpe.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lqbddbbg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2xndxgdgy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vvireymq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2oyqneqfv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2fyummpof.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wwtkrnda.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dmjnxhbk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrtxmhmf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fgsmwngu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2jaiwpsbs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bwioylfu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vfshvlim.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2wlcbopdo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xxmdaezu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ouzhvxwl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iigckynl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hzfkxqrr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2nijhxbsv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2dxxmzqbm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dfbhygkj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2epmplfcd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yjcdptiu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zhpalwfb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jgchxmdw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2wahddhnm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2rwtkeoea.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sjlgravp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2npqpzofa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2mlgqwspc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hbjhnjpi.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2frpbwupk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2kemeedtq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tfplwytb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2slampnvd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gliuwsec.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2rlmhlybq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jpmwjjnb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2rxxqxvwt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2gihnctzq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2yxrpucpj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iskttbrv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yuwioeox.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2njuxrrcw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jqmzwbbh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uehwmtxi.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2cjvvqxgl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ovvcfyjb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2wibcossg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2mqtcxlao.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2rwugkvou.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uasmrlsu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xqfdhurr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mkssexnv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2orgxdjor.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hycvqvan.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jppjfjls.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jvmvhbcn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ztffmwsp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2heodewku.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xxkhsrkh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2szykjoxh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rzxqurrf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xldwampx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2yqzcrifi.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2iynyodox.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2dahjyvyv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2tywqizkc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2afwlnhgu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2isjhcmgi.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2bufzigdt.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ngfmisxn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2asdnkmbh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2fdobktmt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ylllbmif.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2fonquilp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2rudhdhdt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dlvewujl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rdcuqxea.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oglqpcai.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uofswoqc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2vbztougy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iabeucbp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lrvqzntt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2kruluyno.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ludemuml.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rhqmuacu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hczpnwpy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kxwqxyfu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2aozowzxf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2bmqqhxsh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xunqnxeu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kqonooma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mkrcvlii.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2skxcayvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyedwzzy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zlqizlwo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2kvegofdg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zwlerivq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2jqlgyckg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qvcxxbls.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mivtvuri.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2laishbog.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ntrvgwhm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ruzfrdee.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2fupsobra.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2taayfzlt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddowkecf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jqyfafpn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nqclsppy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fwnuzxif.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2uovztepc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2vlyrkznm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ofsiyrvw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jgbbncmi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2nlyspdrn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ipihyajb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rsxwckfd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ujxnumir.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ctzquhug.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2otmqpcry.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qyzmgbij.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dsotbzvc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2sziqndvz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2tvtbrbqc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2zpycvtqi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xosogmha.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fmkbeeod.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2knydgvgm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ohdyqfrg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2acljkohw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rtqxlicp.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2alenmnoh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ciqmlrvm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dkcgnzdi.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2azngcxkt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gaboxrdt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gximiwtx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ajdjkgac.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2edespkcm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mmeppjsn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2rmbgftix.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oobsqord.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uhgtymjx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvycyeqp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bkonsvoz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2brhxadvf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xydbkzps.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xxntzhmw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bwzrguxj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2unibtcto.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hpqnxmjp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ytwezykt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2apkdilgi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wjljbxxr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2pfzbypwb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2sloogrbu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2wwsuqnbi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2nqbjiwmf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2weapydcv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2offhkzho.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbykkhza.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wnxrhstf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nxukizqx.html


<!-- 参考信息 -->