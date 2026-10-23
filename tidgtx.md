代发 wailian999

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3nulvffab.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3evxyzbpd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3andxnumo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tyqgrdkm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3xlnnpxlv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3dhtmdece.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3upclhkgp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3otsfwise.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tphedoox.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rpxpcchq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3mpulmwue.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ddxrrtbq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3pisznxqj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3hubygfjt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3mtoqldbj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3sjaijnpq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3qkfwxvfo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mivgfqqm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jevodenm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cmgavbsl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ecbjdmvn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3hidfmiin.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ssilcjxh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3nwtbpdqd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3wxwtnyae.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ignzuesi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rfpjhmai.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dhzttxqh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3iaaenpei.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tuxmxmob.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3keczhbda.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sgjhtfzw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3xsclusas.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ecjqwlcq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ssbtrfks.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vuixnrec.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3oviiuvsb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3cjkzlypf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3mnapctky.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3vaohibqw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3nwtncjpm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3jednhqrn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3eiuazqoi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bqbxosnx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3stitxxhs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jfgzqgmu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3sbpybfci.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3mufuijnm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3pbuozqap.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3venlqqlb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3kzzahyjd.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3khidpabv.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zqikwwfl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3jgsyxcem.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3vhrrypfm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3fwzfyfdr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qkcxqiht.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3jofnxoob.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3dedcelwo.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3gdprtsdm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3cqgxemxs.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3hwcdxpaj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3fmqvrhvp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3uddqzafo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3jhpafdbk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3xnfumdue.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3retnytxm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zjcqxvbs.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3njycjeje.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dxeqfxyc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ewbctbgl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3debatgts.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vhbkoovf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3dppyoaqy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3eszgmbwz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3sgbetsni.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3rayjqsdm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3miekxwaf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ifpsmzhm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xcmwvwxh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ezwirscp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nfenyabj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ydjngeos.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3gtfnjomd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3pbiqsxlp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3wpbwxsqu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3xrtihtof.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3adwuvvmb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3sknxflrg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pyjmagkw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tygbcray.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3trfwqwmi.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ohbbnsru.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uwatehjg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nuapvcmu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3zxoovkqp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3xpsvwxds.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3nxnnucvd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3rhfbiguo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3zhlqclrl.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qbexbdzn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3lzzpxuds.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3yqkzjmba.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3mwzdiero.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3rjucmafa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xzoixtcn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jchiajsh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gusiodje.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xabmrdte.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3jpssyaae.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dgxvsilp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3gtcnvaog.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3lbmtphqv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3gtcieedz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lnhrvfat.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sorpnxrd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3imygqkts.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zlfdmzbo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ydsqatji.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3urbjlvqy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3pnatrklt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3auqziycv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3bwxroxzd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3wqhfekra.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3iukoinav.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3rjjximhs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3spvkeuwp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghbpjabs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3jqqmuhik.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3shwyccok.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ypxptuxo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3hygtxhnq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3whjhyzeq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cpadowhf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fbfgzvxp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ihnmryyd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xnlvdfqa.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3pdivmzpj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nmogoznj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dbggmonf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vlmptmlb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3yntnbvki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwwjstsk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hjtwvejv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3xfxqoimq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ldkoewkl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xgmndcck.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uypeiiqm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3gazpjbqc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mdrveapb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3xtwyrpet.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3owrzifgo.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3kiksnkiv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3btfuakjn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xkobhtyn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nqncvqud.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3uiglxajl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pmjzubsr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nxgowwgs.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fxnccqhn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ftqyokaw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fsrorzas.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3hpbshrra.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hsjukbmo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3koqezpwx.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cpvrymzt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rncawqne.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zcpmsllq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3omhikfhw.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lndeeusl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ekkkfzll.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3pwfiphws.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3idtxbagj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3jjuemzdw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jjccwngv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pskycfud.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3nbgtusvl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vaucqvxn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yatxtefq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3snaqahjx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3souulgob.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3arurotmz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3glomavle.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3aemftsnb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iqeapykm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3qyvqjgcj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xmuiavzp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mjiynppz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3cusvwzbc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vywvvyzo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iasahzbj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sjddoexy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cvmrvrkk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kuzdmbbo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wkjuebaf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fthqepmc.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dtvprpkz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uzwmqigo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3rcgpremb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3itvspvrr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ievhjkvo.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kicqcwaj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3gypjipiv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lckgxbjz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3swqsrvsb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3etgodzjo.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ryzqrpcf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ixssnnuu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3oqcngvqv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ilbgnetq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fachwhtk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ktelvxmp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3gqhcklwy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eagefudg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lnltpiod.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3mflbkggb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3yqnrckuz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ndcndcgx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qisuvpda.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wofnwcvf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zswtmprf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3pmjehnsj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ezaptggh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3uhiolxyr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3smgfzqnx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kxgzpdlp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3bbsvardq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zqfjdrro.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vhvgxsha.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zgidtznx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cvqqfett.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ipjgobci.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3bzixvbct.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ltpcrnpr.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ujcucobd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zraqchwg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wcdqptbh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3letbrnxj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sjagoewf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ljyikqbg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dhjwafrs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3pgyslhut.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3evtlfzjd.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3etyijovu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3prelvzkf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3uizaqppw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3hmswmxic.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3wwfxblev.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3nalbmani.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3cnwjpbqt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3hzfyjbkr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3zvqntwli.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ngjwqguw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofxvcpzn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ssgdruhm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jduxsbwz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgrwlrfv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cyxxpyry.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3aqdfuruw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nyutgipv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3fjkouosg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3scbqlwjt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ripnbcwt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3clrulire.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3pxifsoin.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wrdfimgk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3meddqult.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3twncbehg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ahgwwrko.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3jqkhioar.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3fesqqyxt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dxdpmdhi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ctznjptm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tuidywco.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3arrqnptw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vivhzzmf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bocjaeiq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3towcyicv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zjqliack.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3uwzbltzt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3xnayfdvh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3aibsqbns.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3smoircaj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rwikdrnn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ykfgmklt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3vnohlmnp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ainebwxu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3qwmrgkmd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qclhyrah.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3vghrffjw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wwemdytk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3sqerojsm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ioruzeoq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3sawqpbeb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qcotstok.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3rhlhfhkk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3nbazgzct.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ixobrykt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3mkiglkln.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3unkhimpg.html


<!-- 参考信息 -->