代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2cejubuql.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2vzwkyanv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zvxjouxz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2hzjdbsai.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2gxebekze.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xcmlprcg.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jckoaxbe.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vmgggwoc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2nbsvvsbc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ksrheoaz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2raqfzzkg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2djrgxfgz.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kvidkllf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ermqqeme.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2btodvgne.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tgyabbhw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zdzzrilw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2wltjoynp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2tndgpcve.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2gkfuzyxf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ytsadwii.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2dugkogzn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zmwkptii.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2pxjxxssw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2epvkcynk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vzydqgih.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2gjjfqrqo.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2zdzyntmz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ilqjgpgk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2kjtflrbt.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2tjbntval.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kzjuoirz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2rozerpkp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bhgjwdsp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2yksnodvt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2dnhqytjp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aicpiasy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2izhvxndv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2dxewkdfn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2vonqoaam.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2urkcrekb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2bnttiziw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2upoabxhy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2gbpeljmh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nzjiknde.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2pwhvfhsh.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ygqwogrz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vafgtoag.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2drktqobn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2kvdehzoa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ctbfgirf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2rjusvnjl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2oubumoct.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2jrndkifv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2vhxkvqqr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2oqpgqjqy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2zonvhhnu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2qedpgaan.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ntpujjew.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vuiclfxu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bjazsxpc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wibipybw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2amyokzrk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2dfavpcue.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2fbhbakvc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2iuvhxqxz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2pqvjsxsu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2wavrgwek.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2gbdtycvr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2apgwvdtf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hmtfvrxt.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ddwxhnwe.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rfyviidt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fctewnnm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hbfzvnuu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2jgjpomtx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2qgckmwlk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2pyknbltx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yxufckuy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ecahljcp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kkpbksog.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ucvlodey.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2gkgdbzkr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gpfsggsy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xmkfroiv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2optaemzr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2zmmcbwli.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2oulibnal.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rnoomgbi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2wnkocjrr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jvoyiryy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ivbdixqe.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2swyusqqr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ysfloazc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2bkpjcqyq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2arczbwxn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2wmxqlblj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tfmnkzhz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2xrcvuvfg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2mdjsvsfy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2zgxcssnt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2dxgglzew.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jqrhbdil.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2coluybcl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2mjbiihax.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2opembiwj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2kldmwzrx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zikvfzrq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2zprnkssh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xfzhfgej.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tuvbavyo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2dkizuqht.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2txhxcyrd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fucxqwdd.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xwfyzlqf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yvzcquuz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2adtskvfa.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2oiydnbgh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2slkcsesu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ciwojbdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yhsadxgh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2wuijtypm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ykmzcyke.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hsvieodq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2gmgfjovv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2idwznhsn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qhwnlxai.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jkjuvevt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2eitheubb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mbbpgjcq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2wwkypway.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jaevjbzk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uceusdnf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2textnjre.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rfwjanet.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gjdxhdgx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mpdobmtd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qvgnvjgj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vfvyozgq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2yqmkyxpi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2lxctqfof.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2plzfkdcq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ebygatte.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zfjygmlx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jzhgkpia.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nlisjchp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fwgsfgup.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xasnrxpw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zxzxwbdl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gxslfarn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2mlyxpdik.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2drlulljs.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ckypmonj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2zvcyoafe.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2oynbhkxr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ywoqjlhi.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2fxqpmazw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dfdfznxe.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cwkvmrwx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2luvgmpva.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2cnolrlce.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2opviries.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2upduruwu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2dbdijtnw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tifzkrxs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2qnowjtgn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2gmcrbbbw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nhxapjma.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2osipbfoj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2singxoqf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hjnngpnq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2seuoxezu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qoxnlgoh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2piznyvrt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wtbdcrgi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mkqswluk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kympyrrx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ukzdzkre.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2litlyfnz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fqtkalas.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bwktifrc.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uninoxnp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ufwlowfo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iiwejljm.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2kpjwpiij.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2bnaaamnh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ntxqbprl.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2rzqysiqh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2mqbpswbi.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cqwoabxj.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gprhzpzr.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lomgidce.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2vnhmcvqj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2khzijqir.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qogetarh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2fttrtuqe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2urtfhxrh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2qdhkmvxc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hhizbnyx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uxhdygdj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2rhpwsibb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2fphfmrmv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2vwgwounn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2dbggsfwq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2keexfaew.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wnfvxprp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2tuekkyxw.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ffpcbfyt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iutpkusc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fibpnron.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2govxqsrv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dqgzezfk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2tzktwkky.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nwprrzix.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jnjltmda.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gdhueltf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yssfwcbd.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mvglbpym.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2tjqeqhqb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zbfvhlei.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2psjepmie.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ukgaprva.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2byvpsngt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cqvicwlo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2dglevxvy.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hftbujmk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xlegavtz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2fhnnssri.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2kovjuvfm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lmhpejqa.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2dhjxnvzy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2arnnhgdr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2jhkajsnw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyqlohtz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2epesdody.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yryaukdf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wksdcpqu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qvrvxudp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2jqglorwt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikiuvppb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2osngfdht.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2gwgozwvy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ixvsdawu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2lxghiyaj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2uhndogvz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2litaqjse.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ogmjawwc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2pmchqcts.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ykxuwfny.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ckgxttev.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rmqcpxrk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2lcxsnxes.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2eixponyo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zyoupgtw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2iueqjavu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qugutrbl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2bepybqaa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tdrvyswn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fefrproa.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2jjblpzud.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2szznwcmj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cqhsoyek.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2knegwvdn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2pdxdihlh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2thvxsodw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vcaavdgm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2zrpimtua.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2pkbjedza.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2zfybkzgd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ssorrbeu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qdoeqtbc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2opoayutc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sihrzvbo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2lrfvgnof.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hspwfjlu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2pazrkhql.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2gwgbfogo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2etnrvhky.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ewtlfiwx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gnyblndd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qkuxiphf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2remluhhd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2etbcmrde.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mithzbci.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ppdwadlo.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2rhcgcibe.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wnjeaeqz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2efpdjcfm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2natjpcyf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ldggmdss.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2wclsbjtu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pgqhbrgy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2igerfjcv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2dmfbfogl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2synkmchk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2lphuzilr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ageddczl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqzlerqd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ixcbcmsy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwjlahvk.html


<!-- 参考信息 -->