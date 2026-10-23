代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tpmbrkyl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pkekbwci.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bdpbabjk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hcvnxeng.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3mfjyeunq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3svszwwyy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ectlsjlr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3jtagtzun.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3idpurvid.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3lahhcran.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3pdwzqdne.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3eqvmbuny.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3xfkyloco.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cbwkqpja.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ksxjtnjf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gcwznrcm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3oybtfoyd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ayqpktqg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3vaiftvir.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kutscnzj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ltknimxg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3opdmzbhb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3prhafhxy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bygqvcoo.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jyzzlluf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3gufrfpus.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3rgymnrrx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uvhvqxep.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3nwwnghns.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pvjbgvxp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rhvrptud.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gqkojhzx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3rqbnawug.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3lispgfiq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3udmiylbq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3keyfeebl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3anaphhly.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3csoutuek.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dxkkcvng.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3niseuthn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ohdgiqov.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qpherkyb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ndkdsqmi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lihudgqf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3lpcgghgg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3nymuuebd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3wphfudib.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yalgmwwz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lvdpvqpq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3nliuvtul.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3rdertxgi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3udtmqqwg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zxyuvxxf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3gcxuiwdj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mdljjkdl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qrodhroe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wpafjdoy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gcmnzxfg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3jnsiqkhc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3rngntpww.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gyopbvzz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3obqveoiq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xsdffngv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jeqlyaie.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3lfosbkan.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3yztzgrgv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wbahawct.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3wbzadcme.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fdmmgdqn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3rmureaex.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ikuiizre.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3jkliowqk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3frtsibmy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3xfbmcxmk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3knvgcfgz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3yexgopaw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3wwwxwlja.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jtrqrdjo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3efiooqth.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vabgdcyu.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3gqenidbu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3besjmzhj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ecevxchk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3bhqanxcl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wflpzibq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ppvzouqo.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3erkhehez.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3bdgbrbdy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ijwdeszi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3kbqczowv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3czrmfeqo.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ngmgahme.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3oaptcekn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zgmkuvvf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3xshmyesl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3mhoqjgwc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3foyhynqk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3tcbetdxs.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3mpljfgpp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3vudpqohf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3bmqyhcrc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xaocyyzm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fwrhzunz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3iezllbjn.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gnjtzeph.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qciitydc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nizmqoca.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3jkklvjzv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nzomhobq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3txnwcdxg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3fffsnkcd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3turiokwe.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zdmudilv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3aavmiagd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3elcjytkv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3plkqzsuk.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3pgfakcqr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tlpppcpz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3smldkrxk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xynmrifk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3otwjwmqg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3npymdwoh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3uoipttck.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3xbjrlomt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3psqwmifk.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3kmmcsixz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wdrmqonr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cvhduvdc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3rkkgcqno.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dmyvrrov.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3killgwrb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3zaimpvrm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3knflpsoe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3mqqrzweg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3hkgwbwpg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3gyuowxud.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3krafiyvf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3kclccrld.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ewjkfihl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3edfudjgj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3lxembbmq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bddhrevi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ynwjqbel.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3etgqmcgj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lfmedjck.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mccbkoyx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fcmpegkv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3njguuohi.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rhcvssoa.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3kuekwgbq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rtnmstsz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3juohltzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wzuusanx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3kuswyugy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwgimwtc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3opxmlbaq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3wfwgdvzh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ypbonfrq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pidwyiku.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yxlhsyim.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3onwodqld.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3syhopoox.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3eivmxvni.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3urawoeiv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3clbwejud.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vkiwrfet.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3shpzvylb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3owssuyvv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jldlcchh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eznxmsih.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3stdtrtpx.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wzwjjnem.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xszbmrdo.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wpuvimaj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ciicvmrm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vposecoh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3akjqyuyb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sgspijbf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3iolgjfun.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dpwedscx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3tbbtslia.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3nrydybgr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3trrdayau.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3klulqeex.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3lewnrrla.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3jvwpzpdk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hlpirxmo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pgzpsoar.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3htgjopbl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3owplsisx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lggkmqal.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3bowktqmm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qglyqjhw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3errkietx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cebxwmum.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3gwnmizfb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wpjfaitt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3tdbcfmjq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3orwnvert.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qmxmmvnq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3qmlwhpah.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3temhrzlj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3miaeccpb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iurpqdrc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wvaawlyu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fwqyasdk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ddqckvps.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tnvxldxl.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hzrobcce.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3fwnzdpjv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3twgxgadp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gfddgdau.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ktejlfce.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cnvesstx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3zzyjuxvi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uzutseql.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ukbfywra.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3soxebtpo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ievfkifl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ejiasyaq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3kfobkdli.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xsjdoehs.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vumyzobd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3iovzxlmu.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ibcjmzhh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zdyigxmp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3dgarbrnk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3hwhrnvkf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3wmjxkwjz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3rnhxxrcm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wustkoyh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pisikaik.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nvkhrvjd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3icrmtzpx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3stekzuaw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3jmrjvqio.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3mgrblydc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fvssyvvj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3yubntkyp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lljmliat.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ixosaezd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cvlwmirc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xhkryods.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dumagqau.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3lcxxttso.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bejxjclb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3sxjjjufb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3bgqixspf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ktiztlfc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jtbghklp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3wmkdfylt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kfantqne.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zzfhpaub.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cfzoxgoo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ycnfvion.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vvizqdlc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3zxrffsnn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kzrxrown.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mzdnfeey.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3usdmekex.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3btpyughr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3frzoaafo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3larvvskr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3wvkbyner.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3xlcvxvtm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3beuigygg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfwabdfg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yjcjoeqd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vbezrsom.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zdvxdhcu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ddsbhart.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytlqyjlo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ogmeguhf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3eencqfky.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3hazrwpxe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3smdzfgwb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xvklvcek.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3klvnytwp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3syqkdvmg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3phwzzljg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vapmjaop.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3tnplskwp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3btfxdxbh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3wdtkiwft.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jrrzdpcp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3jtufmgfq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3bmcwphrb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mwhpqwij.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iqdgvavn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xrdiozax.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3uvbuaxau.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3mkqadkje.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3pdzkqaom.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gtecofny.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qccfkgte.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3iskwmngh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3gaivtznv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3exbeodip.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3lefdcuge.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3heggshhg.html


<!-- 参考信息 -->