代发 wailian999

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pfnslkfn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sxjpwizd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3hvnictps.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3obftthak.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vlcvkxwr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qcnxfoeg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ttuwszro.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3fafalekc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3snlrqtqa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3pkxyetxv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kgdohbmn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mkxdtlbs.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jnazjhyq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cirlegfl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3mtffwvyi.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3swdavtib.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jgqnelix.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3chkocskf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mxavqglp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3cfjlstjq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3zytjdoui.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3zaagfekt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3srlgxhko.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qkfmossa.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uhqyvtve.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qyhkggsy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qidwkoft.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zntdrnxk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3stkpcnsx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3rfzboguh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3lvmpsiyf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3mipbmvdx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gknhkbjl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nmcjsnqe.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3sbimasju.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3xlrtixib.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ekusqjbq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dotaawgb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rwkvflwa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xcbxvxnr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3elvfxegv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ncfxaeoh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3twdhzjre.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fcrenzgj.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3fsadvfgf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3jaqcbovq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yajyxkqr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3mpfwljnv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3rnrtogzc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3stjmdsov.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3hhvrafri.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3glsykobm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3zrktqjes.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3nmixkolt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3zjorhjza.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mnqretif.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ktjjiywq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zxkmppwy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3fbqzgebz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gwvdiexn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tnsepgfb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vlfyoxck.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3owirmikc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3blklykdx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3fhwigfof.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3eqigikpb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ougidrgm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dhmrkyej.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3kjfexgrn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3mawjqdug.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tgqprnwn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3lkpbbitd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3fbnpstpf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kydubbds.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ncdhpqew.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jlcxwpxc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3qguqqhsr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3utzxqggo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3juzkrfaz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3minckfsc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3zydvnzgb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3znyppenp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hsyznvdv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fnxwucqu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3trtcgumd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3puikohke.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ftqnqiev.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3adoctqrs.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3bweiudhj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3nztoisln.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bxgrnmpv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sxjmsdwo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oyearxcb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jfhtzjeq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3kedbdggd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ndwdwciz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3vwyjvvjg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3xmqrrkjk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zjbvmgpo.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lqvfzwwr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3bgguftpi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3qrnoqwwo.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fqmcvejp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xwoxqcfd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ctuiwyel.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ahtnfghv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3neckcqbr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3rgwypksv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3zycvvsyj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3lthtzuep.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3migtwswa.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ktqjtmdr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3jindxlfe.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3tjregmta.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3cjsduatm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dsjzuynu.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3meywmsil.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ddkadrjn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3dsdzfjmk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3aabekaeb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3noksjfga.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3mzttsmjj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ioffyaky.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3gskwphmo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3qjbiqxwm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tcysxmmu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wxuaixzm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pudjfiok.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rklzibgq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3umzhcvoh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3rhrwtdan.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vaethzyw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3hbyvtdxv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ugucstvw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3dpxqpwli.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3znafrcgt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ehrjtbab.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3oljvbizh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jpzculzv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ajfgxnys.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3isauxcgq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtxkpcqu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gtotfyya.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3fhqnwftx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ofrjwvxu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3kvgilkwn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3qhebrvdm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3wfqfllyb.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bplezaqc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3whnltrih.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3hpqgdexq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mbhqvrdf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3fxbellqz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3rghaxsau.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3oqrqcrtl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ywyuubdw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qcvhuyeh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3bymkssst.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hbzdbshn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3inmdgspm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zfyeqfaj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3caoorbiz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yemzvmga.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zlzqrfuz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rncmchlv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cjltbuuh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3whemgvbl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3fdwrpzot.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3enpujubc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3zgxvxgip.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3wprcxkbg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3uaihrxlb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3pqwevteq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3spksqqcv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3johwfgnc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lqgmormw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3prbpohdi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3nkthqkhx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3tashnkor.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3yudyskfm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3bxaudsem.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3apklucan.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xlijagss.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3czxvilkq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ucghdeku.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yuscgyrp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3oaxmohyw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gdxkmflg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vyqlegoq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3sesnoixd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rvodtnig.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hrklwxop.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3rzxjweub.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3wupigyne.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3wozsfpop.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3gjhklfbu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ngkkcbul.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3cbhpgsln.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ojfcosqb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kpuikuwy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ffqgojst.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3stdufico.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3azguezcl.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hshzujwz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kxvfabjr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ohuikzyp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3yrattwho.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3algbadlk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dawiomhf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tysjttwc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3bpgormlf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ovpsslal.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3veehxkvm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3edvteihh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3etdcdkyw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3lnncvmvj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qvtosarb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xbbpnkuu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3yejysamg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mipacmmg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3owyfkeeu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xxmjaono.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3weyrmvyk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qhppdatz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3hdisxckc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kodziwrh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fisobdkz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3mmapyoxk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3vmnxgyza.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3jttiudwk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gphktqyr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3hrvnnpxl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rlcjdeww.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3zrgtlsqg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3sbogncxm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3iayuwjme.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3pcyiukdd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qfdyduoi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3svqkcayu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rkeomsrj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qxzwymbj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cxnaqqln.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3mqvhnxnk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xiizrbon.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3elcsfnbn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3iiqoflrx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ccxadhhz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pmnowqkq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3nenciepv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3tbplcbbl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3sagkvltw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3bdymhavy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3kphxiokz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3cfdfkaug.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ylbjwset.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3eupbtwat.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3xpgavllo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hrmidyxa.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qcudqqvg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3fdpvrqxr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3zimyrubi.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vgotwgys.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ovdccwrd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3fwnvmrih.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3wkvpwpxn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ukazkyja.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jpjqxter.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vadlbjih.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dnpaqebw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3jnduvdmb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wvnpfwzr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3djbkvydu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3htpxmrne.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hfvbufbp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3dtbolfuq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pssaqeuc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hfjpwwrh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sngbxtyj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qykogpvg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ssncsymo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3uitebpap.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3zhwvvarb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ghqzbiwv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3guuqnurw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3prydccsd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nvaasmew.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3erfvwvgg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ojoegnto.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ntnyvrzt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fyyqqxnq.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bkiyiori.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uteqjfsk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ynmckxey.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3uuwredfl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pkrjdizm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3lflzrsgl.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ymjznstd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nomzyntw.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ujyejfwa.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jmmsxueg.html


<!-- 参考信息 -->