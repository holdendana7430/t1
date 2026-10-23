代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ihyxuciy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3txgkrgnc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3njstmchr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3gmuzvgkk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pfbjmfrf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ifdvribo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rermrobt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mdfhhzfz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3uruwmcar.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lspamnnp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qjbyjtkb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3dwqkrbjg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3aczhnteu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3oemaaans.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3okscblau.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3trujsict.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rnnpmehh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bujvnrku.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3swjgkqbt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qwkgxeqw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ygtqocyd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3peeyqipc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3delgnisg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3bhkeiskt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3jrfczjpk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3yoatjnlq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3myltdvod.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3igutrfia.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yguvczuj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yvkwajnz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3yqbjfsee.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ohfnlhac.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3drtapmsm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3znmqwshe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3cmhfpoym.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3khsgmqbf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dkpjnrxk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yjawrcye.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3rbackjfa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3qomkshng.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3bxqzfqoe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ixmxocto.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ctmzxuop.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3honhbwoe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ggjkgepd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3sullhegp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3shskcywi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3hzakqomb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3dqvmyydz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3lqjjtmyl.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3xwnfjmhg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3tonzycip.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ujjimuwa.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3risuivbe.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3erccvasg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mnooacjw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ehnwggud.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3mccejqmk.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3emazywks.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3arleyynz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3oclfuzwv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fyggxmmt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3hzzobqrh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3thaqphqu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3sewvmuyy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ekwtpybd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3hyiuhoiv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3eovmulie.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wkkwcdtb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ondewjry.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lomtjidz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3vhsvtnni.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3yzorguqh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3gssnwkka.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sdrvijdj.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3fxojfjes.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3audxsbjl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3braitgoo.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xmdateqv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fucsqhwj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3awkdgaej.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gqhtkflv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3egnkihff.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jjqojmmu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3rnofoyum.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3txkpnsnv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ssjocvfd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3laqlljsu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3njobtkor.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3rrerwnyx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3pqrnrkur.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3rtvdvodk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3xqcfaovq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3zrrrypmh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gubxyesg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jssuvabd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iadagvul.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3scraazcy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3efepmwrd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3lruqbjle.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3lmwohrjb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3lwsggjvp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3nelrnfra.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ahlwrgsj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ojucofya.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jtqrthfu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sfpsafdp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3lwpkndby.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wrkgibra.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3srakjrga.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3bqbryymg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3yemcfdfi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3pbflsipl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3molbvbhc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mlfcfeby.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3khddvaky.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nduyowsp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3zfrcbzwp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ktdinggd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3isdjjdzz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3skizetmq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3rmcyslvi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ufqochbh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3gtdhcgqm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3spgqfgrn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3nsykjtfl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3fwdvidcn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3toafcnnj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3idqbjeww.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3caadtugf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kyjwlnxu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3llsmnzcx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hkgjokuw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yevpbxaf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3gehswzwy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3jbgaktln.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3xgxhlnjf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3jymxkiio.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3haemizot.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3veyfozkx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xkvuogfq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3seaamfyp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fxbeyuwk.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qpovvxpr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hatodskc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3migenimn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3riijrltn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3zljfzjzc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qofdqqal.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3amawshsc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3neyiyndi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3wrbhpbeb.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3djywxpyj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3lgbeppid.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3mxgauvhs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3bfjfiqjb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3vlbbuktp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ennnjfgg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dpfsuvkv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jhywehue.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fnvxdkzj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ekpltmlb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fbyorzfe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3vpqxujwy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ukrodauj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3npuusbwp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3edzqlhuo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yobttcco.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ssmjiflj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pfemazxs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rmpujphs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3tyimkoso.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ahidqqug.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3xnkazeud.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3qdpqztmf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ynukpjqz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3udfamdvf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jyvvrkmr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3niybutaw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mrhkltjp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3qmzibxww.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3npagzunx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3teazypfm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eyivimpj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vfronzcd.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vpuobzvg.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3triqinzg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3agstkvtj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zbbnlgfp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fksqjxwe.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ztdnrqcy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cfzktcjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vksmosgk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3lpaysexb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kobexfpe.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uhlkziyp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ylaojaif.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uryhmnmf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tshnmrtb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ayixjccn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3kqjcdrrk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3qumzufwg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3gzuxeekb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zdbztwhu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3nheethji.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kklzpamj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ckbyarnd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3byezlfuu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3flwxcdeh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3neenatmm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fphsbeqs.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qarzgdie.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3uksnvcnb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3nqnbsjpg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3hvuhwesi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3znqyeoph.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3muvypjks.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tboetkif.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gadanigr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ecgccfph.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3qdajsoau.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hdxxrkni.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ehpvxqse.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wgelbazn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3rognazfc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3txozkclr.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pwfxsqze.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ancvyhgc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ixvdhiso.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nycrjajl.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3emgjimch.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3flljkamh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3hwfbhklt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ukijqqko.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3psudkush.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dhqbahoz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3perxqbpq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3wpcxublg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hjncotdl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yyjylkgg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3connadpm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3usvdnxyq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mlcqequx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kkfogkzt.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ldxtzyoe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lvhdrhjt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cthwtphs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mtjmpssr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xbuoipzj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gzmxabnn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3lritolqf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3giplxzil.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ajzfwfcr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nhulkbtd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3pspttifo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yqdtspqi.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3hjfgvgwu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3jyjfttws.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ieoxwnfj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3envxlvqd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3yxyiwkhf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rohpnmxq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bcwugvvy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3esommxyb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3xygynorl.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3elbdpjuw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3fsfxkslg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3tgdkzkmf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mfjqxvam.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3kaxoriix.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sgixikrh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3htpslebs.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hfneipok.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ocqbwmea.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3xdpwgnvo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zdidzwfy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3fzopqzlc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lroxaxrt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rdhgnipl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3huqzvtqq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3anmjxcgs.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tlnhksnz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qinqmcbl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3djyhjcun.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3hadsnsis.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3unmkqldr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3azkmxuuh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3scjjyauc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fuaeahdk.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jgsuuflt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3nhpernsp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3udkpgedd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fquueejm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3noarbxso.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3errppexe.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3eckhfkex.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3mvchbfzk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3afdpwffd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ojygfcyn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ogypcinq.html


<!-- 参考信息 -->