代发 wailian999

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3wcgjksed.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mcnuvisn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rvvrlqzx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3itxgveap.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wdkwmxii.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3qcltlvma.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ltfvlypp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3sgsfbxju.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3rphwcgyg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ybfajles.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3btygriaq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3utlrcnqg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ravxswhb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qwlimrut.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3mdkucpnp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3jzjcrhgu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3cvbilzkv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3lzfuvmza.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3fgnfytzy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3gwfuwxrl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xchiyyxa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qvcppxoo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wcueukht.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mtfleoch.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3twneisyt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3tlewghkm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3unhssroo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oyvtizrb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ujokyazg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xyrdaiwv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zzlyyqjk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tsmkmbbn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yhrrncmy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3nckrmhto.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pzqkftur.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rcugpecu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3awgfzuac.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3gqywhdik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqwbcbvd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nkglmccl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3imvofddg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3bfwbhdad.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ffpggcce.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3suwtdgxs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3oqfufwdv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3rjqdbbse.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ppdtzewf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qjxhvruh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3lnfxjcds.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xqfrueyn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3basvotym.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jfbxkipi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oqpqvzrd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wabbmqxy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3frzivvtr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3uhsnxydq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3jrhwiufb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3utqfqawv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3zjuojorj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3llwyjwrm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jqlitrec.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hhmauwct.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kieybria.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3okuzyyee.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qrilbavd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3euwsxtwx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3alvbczee.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kzlryiib.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3zsuveoci.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3hphdgndh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gukmeonc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3takjdvqb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3velhaeyr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wjjnaqba.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ihksqhly.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3tiysidke.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xqebwjmy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3kjuklkei.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gcbdpjfo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3zsrwyznu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kvsgpgsb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3sjjsbirc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3cxucvgdn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ulrdzpgo.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ymbpjeas.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zttdswde.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3raplhksn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ghvzbwop.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tglfwsle.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lsynsmzz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3mxfivjbj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eocvmsjn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iqplvmiz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3byovgwqm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qulabuse.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ypporusp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3swppnjmd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vrldhdis.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3mktonigy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3bektbafo.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3kfyggass.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nglhlhbf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3pimtnoyj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3cyqrovem.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3hawmvvnx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3osqpvnes.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ujbernsl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dlschguv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3bllxwgwe.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3npccmawj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3asahhfhq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3joknpcet.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3szsbfarw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dovdljmm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3twcbicsl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kbzkbrbv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3eeemgxuv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3jsgmvjek.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3lqxfgdfn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xkhxhhdh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3zmtaggzp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uraxsddp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3tsjujgmo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zcoprwqc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lhozlcgx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gngasddm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cmomebar.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mypjjkcw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3pbswfbqf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jkeprtnb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lfzztxhy.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jwxvfqrv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yzyzrzqb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fjivhjxl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3uqyjjhef.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mcqvutpr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hvmzaryu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lxnhflxv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qddlxwdn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uhzovquf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3xbwcgwvo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pfuygbgz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jvupplmh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3lcghpayj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3kyiqykvu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jmhxvpfb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3xwuzsnsd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pnhgutpo.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3zhaactks.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayjthjju.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cxflxuxu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wzhalmix.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fnwrwaft.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3unsqycev.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3gfmvamsj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3opvhnhru.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3somvharg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3cteowbvb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qygudkhd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3wknahpcf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3shtzjzct.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xoogtjjo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ribjzwxw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3pjomunkv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yxqdbhco.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3gopbeazh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3nlrtgoqo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3owjlzwpg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3hmuzebmx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ugifpqjs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3uuevlrqb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3lmpywovj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3pnxwtvcz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3issoqfto.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ttfimhec.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lrrnrwog.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3llrinndw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ogmiijzd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3edwgupmx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hgteaflm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3dpgivhnr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3syqijqif.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3hpygvopi.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3suscfops.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ijyipcxl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3vbfmfcnk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3owhpvqtu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wdglgxag.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3veicjmcq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3tkorungg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3dxknbuwt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3kwybyxss.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ywzakoum.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3grblhhln.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3wtmeokpp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ivnohrqi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cisbievv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nkehugxr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yveyuxug.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3yiivcqoz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lvmuxdud.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3euypxtat.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ykidgyer.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3iztmsmqk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3pqomvwvo.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zafnqjxh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qqwbnrfr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3mzqmxpak.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3lqqnxzkp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3pmyyjxbo.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3bkxrrgem.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3nhddabjt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3exustufq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3vqdadvgq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3cdsqyurn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxblkanb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3xeirqoat.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3rfupnivu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3xeowzkpr.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3cpzjnmvj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ipzydonq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ewxfgzra.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cqtzxuxv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uxwuuoqj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3onyrpnox.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3mfkjzftl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hwidzjhh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dhshfmzo.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3grmqazon.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3mjrlscrh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ustakufc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yfykwdrd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3igsczytk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3omqhpgtu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3mxaehwhq.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ujjhufcf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3fluafmfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oefmhfjr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3uqsesljg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yefqwucp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mbmginhh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3akwtbmza.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3awxvmcwl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3sovxyehq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3phiaycpq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lnxxnzbi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ypiqexbg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lzkmaztx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mpybyoyh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3kpwjudzv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3jsbldqxx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjyfariz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvqxeugs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqogqrbn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hzglkdip.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wbjkndne.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3jqodxrrt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3blfsvbbj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3rueacdwn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3asldawux.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wsdqajrh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mhwwpfgm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lxhzzvvj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hacnfnbl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3kgdlrgjv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3udflbzpg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3awjcltni.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3lkqxbowy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lmlcevpy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ghupjelw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3obvsxzty.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xhaepeih.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3sbjegqol.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pfcihszc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3wtygsvmj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3duoclmcf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gwokjnqm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3maupeoni.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lngpcgmv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3axpudewn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rezzuqry.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3opktmxvb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3mnjspjbt.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nxbdzvju.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qjavragl.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3apbttawf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lmtujbnx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nlxllphm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jvdccyyq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3walqpswu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kwkstmig.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mrvtmwej.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ymeidyjm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gzesaqfc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3icrxsril.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tyzttksu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3isbnvndy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tnbkrjya.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gesctfwt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3gvacowbr.html


<!-- 参考信息 -->