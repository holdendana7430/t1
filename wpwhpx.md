代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3rkbaatkp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3enszpnsg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3agmzqdsm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ejidexsy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qruztzns.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3bshkwfbm.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3szzeiyuq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3inihzwfi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jbqvrcmm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fqzptevp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ouxstawv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vlxwjbie.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3zkviefrg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mxqvnxya.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gtjjhapd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wjxqcqgo.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vcwbitrx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3dimmxdxf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3fgvyrcmw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3xejzplvr.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3qdoqouka.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3nmlywvsb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ajpdtbrp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3regafkoz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qvpzkddk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ibostqlh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3poojcsmf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3rqninuli.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3uljrehnt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3uoyohbqj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3nqrlrtql.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dmqonxob.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3esqxczsh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3sfxprxyc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nwmvuthi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mflafoav.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lthscnkz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3uysatnbm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3wtvrekgu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3nmghsfrk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3vejayjvp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3iymxbzcv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3gimfazpy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3vtahdzch.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3lluqlznl.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dzzpjyei.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qoisspic.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cjcvmgff.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3stuczfnj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hkfvhyfy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3juekabns.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3kowaryjt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wisuuqbf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3gpsknrnx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3cfpxjgqe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3uxmnvmdz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3tkkamlsg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3kzxcosro.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hxwvbvcm.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3rycdykzi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3chgtfeys.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wbytqsvh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3zprvqbnw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3mvlchvpf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3rrxddegk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3cbnfaohv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3okgqdpdw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3xpcznqzh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rhytxcdb.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3litjgxnr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xsmbcfte.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3svbbswoe.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qzsobqtf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vkdtgncz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qfpzdmsp.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ndrschew.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3silrzqdn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xeomctbr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tqrjyrpw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3gcilanzl.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fiyajwcx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bvnpxzhj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ssvkuqsr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gnwcffac.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3zhvhscwz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3yzrikxtl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3duagwqim.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kuaysdoh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hjyfzdgt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3lmadvioi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3txstxtma.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3evnhhkkp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3hwtddmwt.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3rntoypvp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pjudnypd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3awahdckj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ovwqpvne.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dyjwwduh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ygaaxter.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3xusdtyqc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lvjojlmy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ndzjaprh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3iuqvdgfu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3iejcvzzt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3sxvcyglw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xfrqwbym.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3pwcjaidz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mdiyfaef.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3yzonfahc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vsvfjygz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3prgsypib.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3eaessvrr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kbcmroma.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3grkesffk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3piwbqzay.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pzuioazk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hjtocrpv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dyvcdzhg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mvnqvghk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3srljktcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbplqawt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3fngyrker.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ywsugcge.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3srtmhhye.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3sfindjrp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3xvtqhrvv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3azaoqjhy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3azixhoxh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3aubyymse.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3wrxjcijq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3bvnffbez.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yhlhpclc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3lhuyajiz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3nvupkopb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3igyyyzgm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3drmxgbap.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ctibnyhj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3skrfqijb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xnwtvmxw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xozomosp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dckcuxir.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xiiysqaj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ngfobqsy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vurmbukj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ojiizymy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nscnpwqk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lmcgtsxu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gwacbpea.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3fxvjucbf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ugkpxbov.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3mbokoulc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pujjyupc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3bxrswthc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3kyqqcijb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ejqgrudv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vlhomjom.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3nejiitjq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vnjbszxx.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wtbosrkm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3efhezjax.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3majdzgop.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3cymclioa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cdpdzkkp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3tuzktibt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tmpliwpx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3mvvgqgcv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pliudikh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ixufhazn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ttukyyxk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hzopsfri.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3bzxjeiqj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3krppgkjv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wnquueej.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nnzebcad.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dxfaabew.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tetloafy.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aysvnsck.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ovgrsipg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3igpmuihw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kmbidydw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nbvkiwyd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tfxslfrz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3aivteorc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3dmcolnhn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3mdamkvhu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ldzhyiom.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3jlpddunu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3avmczsua.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ngisngfj.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lxtwfxkr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kalzuasm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ibvnycno.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3fdyikuzr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xjspwymh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zsxpxmat.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3opawdhku.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3skxlyjtj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jcpkdtaw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3znqcyzjg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jeyurcgw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hbvkqwcv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3hkljftzy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qmxxmaef.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3enwehhts.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hepvklar.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dvrolpdy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xbinslta.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kmuyeudw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3faunpxqq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hgkzyjvf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fkrjibcz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sykunyhc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3rsfkredw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yznueqka.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3okhpngce.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3repykdrm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zuagniey.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bcfbribf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mjsklzes.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kvcpepeo.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3yycsdhce.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xyjwachm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vjtsxomd.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hznpahza.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3kwcppycz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rtwgyzxm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ydlfbmcb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3saqnxwij.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3oexbgqhd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bmwrodge.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3zxmegydm.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3msclzzwt.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ipcfeucz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ffihakxf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3whkujidn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gxcpnahx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gvnzfyll.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kkrvjzng.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3zdujjfjn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvyxhsig.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3kvdumvfy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3gnesvtqt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ajirlsbz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3wwmwgolb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3rsmungay.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3smfxmpti.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3msmjxxsb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3jlvgnylk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tdajddav.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ephtfmem.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hnaaidhh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3rprrccqv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ywppxziq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eizrfxiv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3pkrctzdo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qdgimsej.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3hvrklbqu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3auixenyr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hypcidua.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3idvvjojo.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wtbylmmi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3shwwwbvl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fvbpkkjd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dwtdfjfk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3iyvbfijo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jvhqeakg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ouawdpmp.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ozatnbha.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ongdzlhl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wcyuhmst.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fzozqgte.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rakacyei.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ueoadxph.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3phpivksa.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tkzrlnue.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3zwuyqvly.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3cdjslrae.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3kllgecrj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ybxipukf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mimmpdab.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3klkkyirq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bgvvorvr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wumlytnu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ndhfobig.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lqljanwn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3vmjvcbry.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3jbuduqkp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3onnmlbhb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3styacopj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mcyxpxmr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xyxdadpd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3roqwejen.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3owktmebq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3dfshbauq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3fuxcnmvq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3pyvztvgr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3wxxeibdu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vycvykpb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3zqrszjjb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmtmsrzn.html


<!-- 参考信息 -->