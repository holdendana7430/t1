代发 wailian999

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2upmepxtm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2qkexaurv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2fbaqwqll.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2qfnyjhaf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2idchyzfg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zndejfoh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2uwfdpmdh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2xfwyhxgj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bhaccqkh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zelepjif.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wzqnkwgw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cqoguryg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2tupkqwem.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ishodrhr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2dqfqfzep.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2pfvcfdgp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mfgkrtno.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ozynxmfr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2eldvjblc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2wrexqcwr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2xgaezzfq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2uuaotacy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ujwqmxzl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2fkhxxnud.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vzelfigp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2pthstajb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jnsyljuo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kmkgcnkm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xxkfvurr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ziuibmew.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2mbekcqvz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2saomfdnm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2gqaftdxw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2jskfrmwz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2vlvgucaj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tprkmvww.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2nnlyhwvk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2efcflfls.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mibbahci.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2xjtanujt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2akyacmao.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2annfbpza.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eiuokppo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2lsqoelzr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nfvpiuwb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tgengmlf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2malbhjdn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2muillhtw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fahpxdsy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2txmmeutk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mgkblhlj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wexstydi.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2dolffvsc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2cpyigkqx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hyngrvvh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qarbiqdf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ndwwjstg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2jjnfozbo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2vhsxhyyd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2eiluzbaz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2mclirbbs.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ghqsqjym.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ijqzwnjc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2sieuwlgn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dwchucps.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2htnnlagj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2dtkyzobe.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ssargpbu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2otvitapq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2cqrsouqe.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2fxyxlzvw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ckbqotdy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2zlvxridc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2stbdfuat.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qkrqxrmm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2txeavjbr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gnrhgufw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2siwdakeh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ioygwrop.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2qilvvkok.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2cfquvmkf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2mridezky.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mxkkpfmd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2qccqrsgt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2unstirjc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2louihmwc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2pikgcewd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mnsgtttv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2sajxamdy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zegesizv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2jtdrpflu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2mfyztrxk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tswukhqr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2dowveizi.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2gnyzvitf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2wnnehwfn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2zithdpig.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nychuwby.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yhcjbjeq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2kmaibzzg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tklgzhap.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2sicfeuls.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2suktqxwh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2rkcdqsuc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2bicinlov.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2mraorngp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2aoinnisu.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gwruqaon.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2whjwgooa.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bbfwznoe.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2obzgxpan.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkvacujv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jcqvcrsh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gjjdqmlg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2muvjtvkq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2pxttykgn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2usixetdi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2xharnzww.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2dmorzczv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2onwochzj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2oivwoidm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2fnxfuzki.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2kqnewcez.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mohoepwt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2edolsssb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xjydpmuy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jegvqhsh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vfhkaawa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qetixrjx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2uygoykcc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2autiqdgw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2frhlugxx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ppwrdeyn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2irzqqxuz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2mijmbizs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jrfhoixm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ywqcfxlz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yiiujruh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2pwliejwx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2dfyzndqk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ymuzzvnj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ghccjxnc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2blflisxo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ltdmcerf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zsrgmtho.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2zmbhqkxz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2clrtqide.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vhwcocbm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2kwmjyftg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ialznvhc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hdbzndcg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xzvrmdgl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qfyawthk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2spwovbil.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xllzzyuu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2twvxijwx.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2aledmjej.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2awlpzasa.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zpdakmdp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bgevxesc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kuuplufk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ezibylfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phfghqpk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bihprhpl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2zequnnls.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2evdpmggl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2sbierwwu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ncnnpdwz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ctzydidz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sxgqrxdh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2uqldhoaf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zubhmknc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rumigwys.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nlhtiyow.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zsnjatvw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nkgpbymk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2skoljkko.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ybcujfch.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dsdyxzvg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zdteqbcg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2plvnuwdf.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2aqgskedc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2hhokrflv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gfbamadk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fgqrsifo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nytdoeze.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ysfyhdpe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bhfpvqns.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2xpdogloc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2hmvcffjw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2bojepvic.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lzpmjvup.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2jxwfsrmh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2xzabhdvm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mezohjqg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rgxyqqxe.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ophvqebj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cjegjqcw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zwnpepoc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xnugwcfs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2siydvuea.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2cywrmrid.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eatxnper.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qwewaxgu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qomttcwo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2esuuydrt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2xclxebpp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rqjpufie.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2dlijzjrd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rginndyt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cgdvohrx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fwrafdrr.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iwhmzrqq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bjzxrwun.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qpvgoxhw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ukdncgtk.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sxrkgdan.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ndsgpzsd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2zbysmtro.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mqylvynr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gplgjilm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2iaffvirp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jaetpzaa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nfetheqn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2htiyhmmd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2rcmudwdt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2etbyfzlo.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2saxnrkqf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2uvcizdts.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hbyjkvmg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gvstpydf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2irtmmqtk.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2eelmaagd.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uymovkfk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mmvwszaw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2fuakrfpl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ucdqbpuz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2cixcfggk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ehmkasom.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2icyvjjwz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nlbotudv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2zgoxtkhr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ybkorhhf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2sxaixvlj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2tnvxbqxm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qmcbmdxq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2tfgmafzj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2naaznfek.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mcfaeatm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2uljzlzzg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vvyhxpqw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uusrxgsk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2hdkysvkd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mikisinz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xliuwazv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2isibqhjq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2krhomjmt.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2klnjucyj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2wyklptbk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qblisfan.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rmbfqdoq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gabqsabm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2oroevtts.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hxfagyge.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2xzhkrbht.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2saauojkf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fzcmsnqt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2feqlsdte.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2oinnewup.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2phguwtvp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2bebvlrqj.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2tkoqlgoe.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2fpgyjrli.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2umkccllh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2iefskggd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2iwgewijx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fsksijik.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ehnpntep.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2uzibvvgb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rgcrtvtc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2dpoywvey.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2qrsugmzb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2lfhsktkl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tuciemwd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2btomxdta.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mydczluu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ikptyerd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ddgqcobt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mgetgpzo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ncrurujp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2pxyrcpto.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sccswhuy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2pnvbfxhv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2gfabyhiz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2jpgqzlup.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hvoobkur.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zdgzbvnm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2koyxisbt.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vebmmeai.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2jtufyehy.html


<!-- 参考信息 -->