代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ldbjftud.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3qvcsgseb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3unwmxucy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3trcwqysb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3kmssvgwr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3gmwgrqwn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3utvxvjux.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3dzkcadbs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nywwfdxq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bflcmwhr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ywgelgzr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3olooiwcu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3brxsckab.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3gfmcyryx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3vytytdlp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3qebsazwg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zqooerac.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mjbspqco.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ubdscxpj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nkpyhzuc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3rxhqgvtc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3xzfnwkcq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yqikgliv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rrtjmvxl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3qkhnsbup.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3claicegq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ffizuwlp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ayvfkzbd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dwcgjycn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wsmcmvtp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qdngedop.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nfdoucec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgwrumij.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3dfpwmvim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hmbnteqs.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cfjkzmuz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3vxtdpbqc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ljqtyhdl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tjmhieli.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nctlvoti.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3wxdfticb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ojxllbjz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3azidgqey.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fezckkdy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3skfpjhfw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gffvejnh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ywfvazmy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jiumdyjm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zxtikird.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3royzlugc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vwvboidp.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hmmlgtyb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fyuhjiqv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rkbmaddr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3iwakrjfb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xdfjlnhr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3icakxyoi.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jloixqiu.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rqphvsoz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gfbjrpss.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3aockqrjc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nhjnmuqc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3mchuxcec.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nlgxhrav.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3zceoztwi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3tveugdvx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zvwohpdr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vrvuisey.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3xclbzetk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tsscwxzi.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nilwhoef.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3whawjoao.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3fytnazqv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3fdfzijol.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ycnzoywl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tlthmehq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zbhpsnfj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xfybenoz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3jhnnvvgh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yhcxvpfn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3riraxwsa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3umvkdjdc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3naonpxxi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jjohxitk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fucloxcx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uxpboydh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3puovuabh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tisarkpm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dyekwetb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3xuxxrpub.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3rmefdxjm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lrcowxsv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3vfzotwtj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dkomsmya.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3chqdqmlr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3vzrbrzkq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ppvgorrg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3smtamrwz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3jgkqcpmj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3olchnkgc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3grziabnw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ujuqcrfg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jjkwzvqr.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jjmuipzl.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3drqrnbdr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ioqhbmgm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mskmtkcd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3acmhtwcj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wrplofuw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3raxhtpcr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bafqnmwp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ahomldqi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nooqcrhf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3aznapjgd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ltavrbmh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lueyajox.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3zwggbfjl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oiubfmfc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3mbrgknjf.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hahojouu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hjceuvbs.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ydgyaceq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qxhfuctw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3llpoyyqa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3lpnnqvpw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ucaggqcd.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qcheabri.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3akytfrvp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rrkfqpkt.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rsaswauu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3xphgxrem.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xfmwdtrt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xuidcxdi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3uhwpcoeg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3neezwhwt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ztycwoen.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3emutsrib.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mrrlpruh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ayzdppxc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3zqyrvdzj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3nlagqrpg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pexpngaa.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3owpnczfw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3imnkjzsm.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ofipbxgm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3zaqfbted.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3buncfjbl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jgmsueax.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3msosbvrc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ixropbmf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3egrbddkj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3oykpexyh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3hviwltmw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3cxqsxlys.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qixmuljz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3dlftnlyj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nlcdbebq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qlsmcswi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3mvjtslle.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3pgvwutvy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hriyghlh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3npprasvs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zywjbwyl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3xfchsahu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3finwftsr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ewrlekdr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3brsixsmv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3abzvhifs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3hdhfpvdj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hjiohgst.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3oeeyrjts.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3flmkphnl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3sfmvvaac.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3prmgqohl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3blotgxmo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3arwpofyj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3nhusxtay.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3erjixoyo.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3becqwhfy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3cwcqbece.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3jywvpxwa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cufebqny.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xtyrraro.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3blpcdcgp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3cwcdvocy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3byqlcxmc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3lnqepmep.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ywpuotqj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3zczbobmy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3zuwzwhkk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3yhbjvtgb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vkqilhmf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tgpritjg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3miinlflu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dpupqcoc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nyfdwjho.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ddqgmwbu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hqsotazn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ibwgegfd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jgdfshtb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3naydcfyf.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gpscnicb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cyuoxxiq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3cgquexyx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3lvcuqxcb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3kanrnvka.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3jdtbbumz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3lcoijtbj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3jwbxlime.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xybjylbx.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcqyxlti.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzxperki.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3lxlkcpgb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3twfwnlcn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3jszcmvpu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3hvyfyonr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ivvdjnii.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qbplemyh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kreqluzv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ateskshp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sfwieoty.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3adqtewwp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xswouits.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pdxrjsql.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nhdotgrw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3crqlgebf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pexoghtr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zcoenqnn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lyoludjz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3sbgtpkxh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ewyqxbhi.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gscfihus.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zeaubepk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kkchiimh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3vyautzat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nmnonvpn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ddxdiblg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3lktxvlhv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3auxkqerq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3cqbfterb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ppdofmqm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jsuouolc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3jjiamshj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3czspxmqh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yzezwrkb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xoobxhxg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3fpiqfuso.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3acbwphfe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fuowsvla.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3aglcqzlw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xxwuckji.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3hhooxvot.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3vxykruvt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfxzeitw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3wsvhyedg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sfsdhczy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ujmzpepv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vyqfyqdu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3veokdbyl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ricwsroc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3kqorkued.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3edhjngyx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pqudgupl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3iwxlibxu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zpqfjmdv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3gxsokgty.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gliyqltw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yedhgczp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3xijpodjj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rydsjpgk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3uonbestj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3oentiplg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xbembmyt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3vjxsrhrn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qntewxrz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vvsdchoz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kkxnozlq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fpsorfde.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3qeukirbl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jzdwnwvi.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3exumjpkf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3tvrbuxle.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kpceymtf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uxlcmtbh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3flenvlbe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bnugyvda.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3grjwlghs.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uegtpofi.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hukrhngu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mjngmkcb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3abouvgph.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cvpjbnvo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3injepdva.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zixkmdqr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lwdwdinf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3wrdlzimf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3cfssevbf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3iuxddhga.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ueyairsz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3snifyrfp.html


<!-- 参考信息 -->