代发 wailian999

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tvqrtpnm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2jgxpwepm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2abedwhrl.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ulikwqew.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2purvfjeq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mmfpglja.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hlafgeul.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2puyoodaj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hsrcziml.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bqsdsilo.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jpkbrnpq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2lwcbmjlg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cuyqelql.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2mervqdsx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uhqljdix.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2gguehkfc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dpctooaa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2jqfponmy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2uhhpakad.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zitzosib.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ammesrmh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xmfybeeo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fiwybxwv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dgbxutzn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vibsfbxj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tmhwwruw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kryrzqtf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wssgjdaj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2sbbwlcbm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2whsgyxtw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2fqkhkdly.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qrwsmpwp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2znxpvpcw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dyxajkbl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2kfrveaux.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ywlavmpx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qynbkohu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2wcdraylv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2amgelprp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2txhfzjbe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2uzftuxgw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jzpiqima.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xcnzmlyp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2razpcuvt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2dajvtiuk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2keikeecp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2rmfwnuke.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kpvocbxg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2vwfoeasm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2obbkfvlh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2redptyyq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2aoccucpu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ymkcxymg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2emfyjvtm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2adlpkrht.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wedaxeyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2slkdmyat.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2plxnldel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2suzhlbus.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ojzobpdv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2aedtchyg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2zxyoxwtw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2smjjpfzf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hernfwpi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2sguafrdb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hntofynv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2iacwykck.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mvlqroaw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2nktrlojt.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kchqixqr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kjszclcu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2aymihora.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zmoubaiw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dmrcfggy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2quiekjjf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2repukkxx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2yclpbrra.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ijytkitm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2vrpxkfii.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mxmhifgj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2czixhlyo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2esqayuje.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hsemsxlb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2uachitil.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2taszljsi.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rqvkanwa.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2wftxixil.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fvryvhnz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2bdrbhoju.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2xlwwzipj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vijmvztm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2feefeyjl.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2wxlryxzi.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dajmbrtr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wyjoyjjm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2dznxcfms.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ijbjwkro.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2dpyblzsg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dpbrdofv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2swxuefkh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fntzaaii.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2grbtpcfk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wccyagsm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qyetkqwb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2vnrrfzhu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2serfrtpi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2cqtpwopt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kgpsdtza.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gzsrsdpx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uweusuib.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2avfaexpz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oxtpxqop.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wckdmays.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2brpxsioc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2yytygnyt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gttiltgg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2cvnnmkvn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fjnbzuxs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2lvglbedp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wglkaist.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2rakqumkz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2iiakztck.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2wfrimeja.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2zgvyrtsz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2wpqlytxt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2eejccojg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ubajdzgu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gsjmkrvp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2trrzjfee.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2phgbbtkh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2toswbwiy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2dymhwgko.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2alxuxbwk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2woixkpmw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2avaehhdt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cwynjsqd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ybqxeico.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2cupcbltt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vjmlydoa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2poijgcjw.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2rkzzhzed.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yrvuzdmm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wsroanyd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cfvhxacb.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qxlthttl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eoelralo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qjvpvqte.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2exkrtyqq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2zkmnlebi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tmvyrncx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2aazjtnxy.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2saumhfhk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mteaoocz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2icydhubd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2uiptxotd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jpnkkcwb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2aecnkuhp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rwtwocxp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wvyzzook.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2axkcmtei.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2mrwsjrfh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2trmzwkse.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ycwzeoxv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2bwspoiwg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xhjfaerd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xrcnelwa.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ggbglscq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qvxfmpzl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2rjkakles.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2husopxtv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rloyaqmv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkgefvgc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttioaamo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2forbstqm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2qjjhsshs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbvyqeyc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2iyjtvvuz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2uaygewso.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2pvsdscfl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ldzhqlaj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2yrusbaza.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rdlitvxy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2vglpmkdo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2lqrsrvpd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cevhouva.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ndeeouli.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2qluxasqj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2aqlzgjbb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ntrboxqa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hsqlwcuf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2bavwkipe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2urknfymq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ddpbzvfh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aluimijg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ezjdicdu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2jcwgxrpn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2zpykwieh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kiivxuoq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ryauqolj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qcdblfwp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2zlzhuwrg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2xztxsvnw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2uysksmij.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2shenunla.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2rpszmehm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2jlgubjag.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ylrhnrev.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2sxpfuont.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2twhbikkt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kohflrha.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2feuntzxc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2wewwrvbq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2aezihrvc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2yzgljkoi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2urygujen.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qzmsnlbx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cagojneg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fcugjmji.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2eauqpfwh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ydlvavze.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ceuvkbnb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2xqnbmpln.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2hhahdutq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2eubrocwz.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zdmkescm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2cbpqoqgp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hqsayscc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dnxtjpkp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2itpuikfl.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2oigducss.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2qhtcqjri.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2mnzayavy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2mepovgun.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ypbncbao.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2kaoqwpik.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkauiicr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2wtjqcyke.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2uyappidj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjrdknhb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2owctkify.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2xkymaplm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kvgnctbg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ilsbjojx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zyltwfhu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yiqzeikj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2lbfeuzzv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qagvjvxl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jowctund.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2chvgaqzq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2hmrodlpe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2paotlihm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sglfqmys.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2itunfwhi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2pzlbyubd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2grehzqhq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cuosvfjt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gcxwwkol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjstebom.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2tiruulqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpktskwo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2zwaekpel.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2itbwlpxj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2glfuzswx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2mnqfutzy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2alzdqama.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2idfxwszi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2uubfghdl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hpgsilye.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tpkabmnv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2zabpkmom.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2nwqsmnhn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2kpzcnrzi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzdvseph.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lweqjscq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2pepzccad.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2rsevgfiv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2zckgoabj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2wvtckpez.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2uyxbmpon.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2onryliwq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2negltegt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qimkunhp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2psmoqubt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2cxsjxfjh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2kmexxlsl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2rtsemcsw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xpiaczza.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2saechvik.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jslxpxwu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wbokmgfd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nnqglyqx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jdqqoric.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2pqntujwk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rolkqndj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2kxcyzpsw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2urflhkfa.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2alovkhky.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2zgvyovpr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2snymoezh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pobqihix.html


<!-- 参考信息 -->