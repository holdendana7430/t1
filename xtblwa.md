代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2cagarvyk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2lqnkgoaj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2fekrvvzx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2duhdpbbz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fxtqerdk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2bzohfvim.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ramzxnqy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2pmzfteod.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2spqijaqi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ctcfmsua.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2xkvmmgel.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qwktqkhq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2weiaprgk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2aqbflmjq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rijrvvmv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2buzvkhxe.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2eclpbmqx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2qveykqcu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2vhcibhzx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xwjxsdwn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jcsftupy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kjctwmkm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hsedvuog.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qpcwtwvc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qvtjwuoa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2oqobqyuj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ixomagvx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2nayvydcs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2wxgmqdsd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2oohcamor.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2xbqvcxld.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lmmwsyrq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2psgihpoy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2phycdgzr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lrklutql.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2kfzhznhq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2krvbsiul.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ikdmdikl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kfhvqtni.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2skjibfqy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2oqmsthjh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dquuevnm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xudykdui.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2yzgyqwpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2suptmapi.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2pycrwpub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydxvsqbs.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nkrvmgpy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2iundlphb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cwiyvgnk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pgcqdfuz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kjoqbstm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2mllyabox.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ydkfoyjl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2khwozsnq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hcxckdpg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yemihzqb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tnblutda.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2jgxfluoo.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pblueeir.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zbqnygzp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cxomvhlq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2otvmnovm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rpmbqfae.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2etsnmyss.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ymrewfao.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2izizszdw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2smgnxsnh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hbluoizb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fnlswhtb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2etbgyqed.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lpatugxj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2twabhuky.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ehkzbtfi.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2lkjvjpdm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fvjcsjuf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2bjxmavax.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2sejiesxp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wkjfeggl.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iwajhqsa.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2iorpoiej.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jfnwbfko.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cmnkhmbh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ycrqjjam.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ksryrswt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2vnurquem.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ncvxqbxr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hgzmjqnk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rzjrzjot.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2azzfhwru.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2nalofoac.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vjwkrjof.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2suwystnc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2torcmbmf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gflspbhy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ojulsqhd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cezzdrvd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dpakoesd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rzytosqh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bfwopgvu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xymaaowu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2zeutaphn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2xrbesbas.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2puenurrh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mtsfmomy.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hieihsqp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2cwvozdts.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sydaelyt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2vrnrpjah.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2krvjgorp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2xtdyvlca.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2nezcfrbg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ebhkvzqr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mykeoqno.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ivbrlkoz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wragjxvq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2uqybqkev.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2okhqblvn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lrueyvfq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ydwaqwfp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2rmuemgzx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2momwnkew.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qalpzgjg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pqacioch.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lbxvdnsa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2lqzapdcw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sfiktetj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2buvhxuuj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2uptuuvcn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xzmqhdxx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hrzsvfab.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hqbwpiaa.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wsmnnpsw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lnkkwrth.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zqrfpnbl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ccqaefae.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2oiufxjin.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jalpidym.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vgvbqics.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2okksdlow.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zbrvyeli.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yeytrnpt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2qxfshrth.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2sxdngkzv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2bytasbsp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bcvdzrpr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bkneepyr.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ftseluqp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2hndlztgl.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2miyaxmzf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lxlbwvqu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2bwapaqpv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2jkzgiinr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ytzdsvid.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2enguukfe.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qojjdsqk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2epzlbove.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhoiegyr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pvecxcok.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2asyixarj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dfowebkn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wfcmtsdt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ggoxybbh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2oxlntokq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2eghsrlgj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2lflvhwdw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2nashcbdd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2wdvixwpu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qrpdkrms.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ufkptwhd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2nrxhrozw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2idcjchuo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2imufcera.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2frwzlvsb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2fnnztoeh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ghmmrizg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qaygeymy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2nsgapkmm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2zpdgapla.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2pbkioaxz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dnoiuxne.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2euevgxtb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2mphpmscv.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2rjcpvbex.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ixhfwprt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cvhcspxm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yhjbgemq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vnpklxxa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2grunapkh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2doewlmll.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2hnbismar.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2jegmfnsf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nlmrbqyt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ponbyqki.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ophymqat.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rgjyqbti.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2qahvpuza.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2hauvwjuc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2epmuxvll.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ahsslaon.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2txruwszv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2yqktjxtq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2nxzdpphj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ynevnvta.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hybayfvf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ogejasut.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qrjsnwip.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2pxztlepg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xzzvnnjm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2prcyxoiv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ujqpcnbp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qqowlxdt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mxngqubt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nfhzljur.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2budgmqbg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2rwakxjwj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2xomaxvvs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2jygeijtr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2bxtlymho.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2nivmjoff.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zxcxgenc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lchsosyz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2fhmisfad.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hbijtpon.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2rcnhrehn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2yfvzxfom.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnjbulqa.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2fhxesbzj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2pvekbedz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ifplldyd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gxkinlos.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2etacndxn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jkxfwkfl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2spfpweqd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hbaxasak.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mdehjbxp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ztnrylue.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tmbgiows.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2draslldn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sfibzccg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cizgjyop.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kzfulmqq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hgersiiv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pdabgadt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2znvjqqce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hktheumx.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2nqudvgtj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rctiwyyi.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mjkywltg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2plcalxhm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jrudavyn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2aoyamoqb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bmtffoul.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zckavlys.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2tudwuxop.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fbgucqng.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ylqcxjbo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2kbxhlwvk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2jhyvujfj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkicapau.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xgxlqzhi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bturjexg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sijylvye.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2fvmbzoqv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2hdqsxrcq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2kiuwpdvx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2bdgtjxcy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tspypdsw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2koefkneo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2suftryff.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tihwpali.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ivyoimdz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2yylxwtwy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2mensjmfq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2sbgrqejp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2iwkiajgb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pgtzxzqg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2syjkxduc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hyisrfpg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gggbvahd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2dnlxkyyh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rafkncbz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wnswgdgc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2vimkbovv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2giqvvlef.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2sesykmsg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mwnydouh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2quwvcwup.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgltjtac.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fmshplnx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2xellmabr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eacdojzo.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2roygjznx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2maftcbjs.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pbqrudbp.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bbnirjtv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lbnugcdd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ihnyzlie.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kevcgffg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tpayvwfa.html


<!-- 参考信息 -->