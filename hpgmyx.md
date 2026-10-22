代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oszobaab.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ggxhnemz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rxabrxmt.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2elclnrfm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2moeryyoe.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cifkgedv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qjsfoxdg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vdzbbzfm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2xombwabc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ucrqyvug.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2vnoxrjtu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2bldnwqmb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2qkrggeaw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rsditcxx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gavfkqgy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ebafixij.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rqpvdqss.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2arnagile.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ubvothyd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2rtbtjnpf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lkznfkqm.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2uuyqdiax.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2hmekfuca.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2grixptzz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2diiacgbq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2errbmqbn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zuruwqvm.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2bwyalvpu.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dcyovbmc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hmzuwrui.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2kzpbsxmn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yqvxtucn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ydzjtkuq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2axmtlqja.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ywxyrsti.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2mjtaxmhw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cvrxedpc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vdmxmlvu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2aoszsmvg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qodybmus.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2chpkvkdz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2kvjezvya.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2oiczmryl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ligsdreu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ppuqhwcu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2sstepjbb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2hlqqtprm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2mypjdgml.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2yzfdhtbr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2pgdwmxzg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2gbmxiymu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2wcnqynhl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jneazxsp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jhmfhhdf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qhqbqsye.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2teagwcqi.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2udhosmod.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2jzrpzgyz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rpmjurrp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xgnrkidc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dfocjxrh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uwgslqra.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2lzyirfmi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eyjrispy.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zdnqxwqw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2xojhwtvy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2nvtpgvbp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tyegmeie.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2laqkcbjq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uyqgnwqr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2woiedesb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mnmbfpce.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2mtggzvlb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2mxmgtlir.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oyjlrxih.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2kglbdasb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hyhxpdpq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nvlzzlql.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fxpsfehg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2rokkywwk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nxykncru.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qocakskp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rjgpskpn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ecqlvkfw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kmwjoagn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2alqlqgyk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2dvthucim.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zmzxzwza.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2iyvndjzg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ksyjjjit.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ddcbrdau.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2txpmarzs.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ltcbomne.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2zlscnlon.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2doxeueuh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dcycxnjm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fsiryeoe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bheambkt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2izeuqqrr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2vvsjqkbj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vkbwtxzg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2mkjknnfl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lqahokbv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qscjzxci.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2tlzfcvps.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ikdoifiv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2srucikak.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gnupqhbw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jqrvfxnk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2cgudoffr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2pzopwffp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ltyhcdwi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2zvjhebff.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2lwyyerbx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2wjowvcaz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2zffrkpui.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2xyetcbvs.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2rnbqixle.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ftyzvwio.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dvvndwys.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2vtzesglo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2smqvmkdv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2obvjlksw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2nfegwzxq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gurmlchy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2tbfoeyow.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2uaxzkwvn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2yebosknk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2cwwpjjoo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gyqlptji.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nnrvbaho.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cxxkwcao.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kmbjttcd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2iifulibv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2boxtpzgr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2nbefovef.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2cnjbsgzu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2sxnzkccf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ebkyfqhf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hnjpnpnm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2yrskphji.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lixsascl.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iyqjruri.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pihewczr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dkdyxemm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2psnpdbvi.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wtotpkfg.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ftznaaog.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2jypcdwmu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2dwxlbesa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2tcrwiiyw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2nycaozoi.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2fjrepsci.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2qirtstiw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2jrlkmtlp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2vuqejtlz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2phuoghxu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mgpncptu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2nbbgmloz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2viccsxwv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ntuxcwiz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2dvwuyqei.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dqopusfj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2sdhbaurb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2cxiqctag.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2xbupvlsi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2swbzjlwy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2quductov.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2vjwtfsqa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wbkqupxj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xevexgmi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ajeuzqcu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ffvikjaq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2zmjxqjgk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ssdheowb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2gwcrxstt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jfpfzcgi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2scimdbej.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2xowgffcm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2keqncscs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2uxgbxmxe.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gfsjbzpf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cmsodwrd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vmngigbh.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2elveblro.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cqdugsmc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zccewfad.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xwoqqtja.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2yhfzbbhf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fxhckzqp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rweubwkj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rigcceds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2peotjphl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2xnvrfgnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhnnidwg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gpoefgad.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2gjlujzcm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2vwqtbjqo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vzsysolp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ikinvmou.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2frthwmlp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2iuvfumin.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2rnmnxlwk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eyduwxul.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ogwrnmol.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tqpvgngx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2pchqfkoe.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gqthjafa.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2banuuxly.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mivgeewe.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lzbtamdh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ttxalnbk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2mabzkpwv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2yylgzivh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2iptdvpqg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2midvuvkr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bqqdfbyz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nwqjdhxq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xudrapaq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dumccbxy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2emgkfruu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2opkdpvuw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2rgzyjzoh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bzlflgwy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2lgwvfgns.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2cakuajbh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2djchcshu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zquvbvhq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2yrpxmbay.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nievlmgf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qfradumj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2vhtlrwvs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xwspbjdc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jllfitwh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ojgujzmu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2wsajynbo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ngeajamm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2fhdtnrpn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gykacrec.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ycgdytoy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2hqosqscy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xmvmcjnk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tiqyvovt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2islxqvpx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tgvetjfe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kjdofsrx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xiivnzsa.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nphbtfov.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hjpyojii.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2rtkjuaip.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2omjdtwlr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2koilkyya.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dtidowmq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2drsiabyu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ohyerdkx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rirebdlz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2tsauhgqe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qtfvziqb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2nytrulxx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vouujduy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2gtsubclo.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2grbwkgny.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wbwrurgt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qhjidhod.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2nmtvztot.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gmzjsvzc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2eotqlxya.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2onakxnjb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ccvenjnn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2boesfrve.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zomkqmyi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rgpuakzy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kwpuwgoe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2nhhncggn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2pxwyizzi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wgflrnkh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2dikpttib.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2veinqxja.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ycdexsre.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jzszyoso.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2faxnnsdj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ycwduozb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2takbffty.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kqtpqyxw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2mshxpttk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gqqochxb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mnrffhup.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zrkdthev.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rtlsltdt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vvmekbgp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vdrokjic.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lxomlpbs.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ihussqzd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2yeadhide.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2gfbhysxe.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cmwueeyu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2trzwwgtu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vgxfrcql.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ehwxfsrj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2umgsqqxi.html


<!-- 参考信息 -->