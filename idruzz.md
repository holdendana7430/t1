代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tqywzeab.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rxzcihpp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3eqkehigo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3bfgvbbar.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sabnowla.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qjrnrofd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rafvnaiq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zwtzrxbg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ukyvkujc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3bkydocsq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3iktxwrfi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3urweqvgm.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3pdvscpjy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3oljcikxs.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3egeztlow.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3riqueqgx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3dxiatcso.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sxckkgqt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3mlmkimpw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ryeffshu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mjsvqjvs.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3guitkhmn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3xaukhbmg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qaudzppi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ljpewtml.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hzuntpkc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3mlgfahww.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3acrgxjxr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3htpajntf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3sruvrmpf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3vxhwypxn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3bufnkeqv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gjofqjgx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rhyssowo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hxpnwclb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ulyitxcr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3xteofrlv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3lbzqtfsj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lgmtugfh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3lofgqung.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3bmvqbgze.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pkhougci.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mhwuksxf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3oabkekbz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3zpriqtit.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3pxjdmdkv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fxfzitua.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yvqxmtmn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3orgrbjxa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bsttvvvd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3oqtubrdt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dugyszra.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qaaiixbo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3pahiplyt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3odousmme.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3svkmyjbg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3llitrjni.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3tdisshah.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mivtayuv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wddeneuw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3puoimfez.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hkndselr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ybivabrh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3lifgwmsf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3mbctjobn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3sqsajbgc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ilnqgvma.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gtqjsezi.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3clmxhkxy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3wxeojroo.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lekdtyrm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3lrdphvxi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yawrcslw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ofgtrsyz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3agasvaji.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3jemfeczv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3uhifjvkf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3dbfsnhhm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3muiotyjt.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3vfdeihln.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3jnbqpcbm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qpsaujqp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3bxpvfvrs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3txlywpkq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3vgfkbwhx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3unnlhntx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3btbopaym.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3zgrkbsyq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xhlmhvmj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3huzcagtj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3runntxbx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3zfetyins.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3gdmqekxp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3mdyepsus.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vroereaf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qozuawfy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3dkveraca.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wmknzuzs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3fjisnltq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3kdioheqg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3mqisbrww.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3kcdytfdw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3qciwqvdz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3mchoyaej.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dphujtam.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uwqqzode.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wapijvbg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uocopebl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jxpbzulp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtawfygm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pgchocmq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3wsbnwyer.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3urjlllbr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3meeghrwf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3aducybds.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3fudmwwne.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cvurskaw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3zvwcxogj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3zovzfqme.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3tiosfplj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ttwkgipq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3bksidnvy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3fblhstwb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xjdxrgex.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ufschwrc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3nungtxjz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3blohknwv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3uytshmvz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3lyfpfuno.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3exngosye.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fasoetoz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sfezfhta.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3boeggqgb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kcanescd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3iqiaiwrm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3imxdizoj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3febftaeh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3pfnowhoy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3wtznggkv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3cfqrfcbn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ujnyzhhz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3gujxtrxu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3lzanuvnz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jwmenscx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3uupwfzbj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3cmxfqzbo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3gtroxsyx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3htteareh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3unwnsjar.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hiwuytkq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hgydqffa.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mmkfdaho.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hphrhgra.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3jzhnhmvh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3imsczbju.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lpgpufwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ylhrzkeu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3baysitrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbyinvkw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fpywnfms.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3uzswmviu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ujbxkgif.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fakxfplt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3pyqnapef.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3koszilpo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ntdzrqps.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3cohdqsbd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zxkrbkxv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3bzjrbxxp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3axoxafve.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3kevblwqa.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zmrybgtv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3naufyldp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pumudegp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3mtdiksmo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zxzcunbw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yfhieoye.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zqearcrl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3qipfawyq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nvouhntr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3esfvejjh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wrdrrcqa.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xsxldukf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nhszwkav.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3tjechvnz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3kiutcwjx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3gmqfnkxc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hrcsfqdm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3iijrtmwu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3wfhejhmq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cybmwzju.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yynavpls.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3sxlylidn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3pslpdjtq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hyupltna.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3phpkfhgj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oijutksc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3wnbyovdn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ecnkpzyj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3wrmukxet.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cpmxdxym.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ydsqeukq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zggcwgqc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ykvanppr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3msdeeyfn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sdejbsry.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3rvbjtnbj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3smysjhwk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bodtdnqj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mjcltbfu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ykrstvhf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qifrqhqv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bgfdrguv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3aibnlsff.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3lhzcgacn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sbencevs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lfvnzzlf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3exizxehv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3eqhccari.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ycwnnsyh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ngbraqvt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nepmwrsu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3czgfgpxu.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3azlzxhqc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3asqxahgy.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fhrgfafx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rtbaxbbd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3pzsnwvps.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3fmaenjzy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nvicphrf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3izubjftg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3riywyuyz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3swrbuzdy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3qulzgeeu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kyxytagl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hmkodvhw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hesgftpy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3vwzxhavk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3oamqqrwd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ujixglpq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3odulqrxr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tcmbhmvc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3tfqnhzqv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wwistadg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xtpijcee.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3uqczkuzm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ovmxoysq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bqvmnlsv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3cbxbipgn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3tqblseoo.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3yaqscloh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3podlwzov.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dwkeyhhm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ujgfekyb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xsrmksab.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3cqgikwbl.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ehiodmfl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3chrqcbax.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xsdcckip.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3azheyvih.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jpozhodn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qkrtumgh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3elbxckom.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ujgjogpe.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ghsdvdxi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rvesduup.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ybbjxcss.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bonjhqqc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3pwjuytdd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3jjqqvhqi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cfilevpe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3frpdprap.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uciaokey.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3hdpeiwbk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3wokducgl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3llcoxxap.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3frfxycru.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3eoktzgnn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3izfranie.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3kefvlcqn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jzghipbn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vrvvhzew.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3dcbcfovn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3wyrrgbcv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pwmzhcax.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3gdbplnyl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3grvuylcb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3owxeloow.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3bgjghyag.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3obbsokjj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3gkifzarh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvecjoqo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3qpbgkjzf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3stdnvxzd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3tdpqbypk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3lcgpuakh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3kbncelai.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vpggxdkf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gvsubpyu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3uqmiuclj.html


<!-- 参考信息 -->