代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ogconfjt.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rzqltdbw.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3zglhybsf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xgfxxikw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zamfivhp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3qonwkzbr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hsserufp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3pitzchfb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3jpbwexvg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3acknmvqi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kqaxazhu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3hhbdhtob.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3huiyxqjy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rxjanqls.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3pyotfcfd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3repztakv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3grphiyme.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3gqvifodz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3bokobmpg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3cysrepyx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3btznohqn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yvfgjtuo.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3xyrhvfts.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3owfznejp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3umumfdxs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3piodqglb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hvqkhjts.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3seuonfnn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3nwqtnoma.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3kkyzldjj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3yjcwbhre.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3arnvlhtw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3kgliwhrs.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3kqtorumb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3nybkrjvj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3swwkddcv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ybmcpazq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hkbqocca.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vzdexbhd.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3edetrirk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bdjmrjqt.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3zpeqpdpu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ioirzhco.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3bqapdogq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dujwidqk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dmewzcod.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3donjopau.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hctwwcfu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uuibnjbu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3bwwcyxjl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3urpnfrgo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gvjksftv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3kigcigcr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3znicefzg.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3moojsdiy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rrqgpgje.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3bmokcsed.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3pzyyeije.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nwjznmgw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3kqaiydiu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fihzwerk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3moolwxkx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ugmpbhhc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xgjvkree.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3juycscgs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lcyfwthx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ufjpknch.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mngaldym.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3eccvhiuu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3depseubi.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3bokwxzrz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rppqryir.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hlsdwrjq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3iezyrzbo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3tconmros.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3tbxxhltx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3lrrqkmhx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ohuzcref.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dqdngrko.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vgnghtec.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dkwizsjd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ldktyovc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3cpkzmqkm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3jllbqeto.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3etsirkvr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3uohrdfku.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3crimkrtz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3vfxljfac.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wartrxfl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ndhsjwbi.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3vetxffpi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3hfwztxbb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jbtvfiqf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3jttsbirz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3mbklpfqq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ufocjefi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3grnssxag.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3qenobyrz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3xjwyihsl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3dmwsuttx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3exotbbmg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3tazuwnnn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ymtxlwhk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uvmcdykm.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3rvvjczkz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3wkejapfp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3yjkmarwh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3uvkxrvwa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3sozalvza.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3jmqeacef.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3kkfpojan.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3npfyscgz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3kbbvoirb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3qpxjjzoi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kgtrpuqo.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ndhkqskm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yjohtduj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zltvtdyd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3aguxxlpc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3hdpotsbu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jplgbagm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3syqpozpu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3iueccfih.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3yfjxpxvi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wjbiszsr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uqsyecss.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eifaazvx.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zhfbtsnc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tgwzkymk.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3puiwoxle.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kkllmzkl.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3squdnfse.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3orhtcmpe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3bvhstgxx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3esdkjjxq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3mjasogqx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3zkxizhsr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3pkkiiods.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ixazrxsx.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ixblzolr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3foydbgao.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mygbjnpq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uxbpablb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hsxgbnea.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pccclvkr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3jhownepo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mnxbrgxr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3pmxeqtkz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ecpqajax.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3mskafyce.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3dvryqctm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3lcytthkl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ghckxfmo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tkegcehe.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gioquoet.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3tgdtcnve.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3cxnnoumg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3mgqupabf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3pzlbzbqv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3pfvgvaqc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3fvzaumuz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ybiccwzt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ekywkevy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wbsareka.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3xqmhhigq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3xxvrmuap.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ffliffbw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3hyxmqhtn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3otrvtrin.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3izrazrom.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ygtjnfjj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jnvrrdnf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cfjvwffv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ocdlyxkc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wnlqgvvo.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ilsejgjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3behgirvl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ehvbetfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hibmahnh.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qvynndsx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ptwbbyus.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vylmsuec.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rjhyptdq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ygriqfap.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3qmhhsszt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pxuwauzt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3brsahfkh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3inodvncz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3napslbtp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3nkbwsbvb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rfnqbfna.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bfywrgiw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3iqvbabtv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kheblaxb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vhhqaqli.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3meceasix.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3vrwiagfd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mktpypet.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3qoajsuxq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3adgkjoin.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jcswrdti.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gsxgsuxu.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xplzwpjo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ekxbnqzr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3pqdpfoou.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hyfucrvr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3rbkuoome.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3coqgipnq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3cfvnljkt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3xfacqmbv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ddidxxlz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kxinygak.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3yygfmfar.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ruapkfup.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nausuwbk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3rtvxsqxt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oblcaezh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3eszxpyxp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ckdgegsg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ofzcbiwg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cmjqltpe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3bljtvswx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bdmjbmci.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tmfdtfxv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3hhtvlyvx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fqoapazu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3smjajmmp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wrvnqdua.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ywgzsrfe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nxuevqoo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xddvezoz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3brzqpgqu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eqkuluka.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dujighok.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3qnbhshfh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3syvbwznf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3umobgvpu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3laorslfn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3fgfpsknq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3cuhmvlfa.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3jfkecuhe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3bemynauv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3avyzwlxt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3wuezxske.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hrjkfcka.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kgldqtvq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fyrdivet.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3bkcuiefy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3mfodnkso.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kvluzxkt.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3viwwagvc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3zgxhjxre.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jehazgsn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3nibfgpag.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zvnuqhcu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mzdjqiys.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vykckksw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3wgwwqizo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3seifabhe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cbwpdsly.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3slygphss.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qtqaiftv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3asnbyaon.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jmcvfqfz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ebqemtqc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jafsmrme.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lkoyvnrf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bilwurou.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3nmbxzqxd.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3sfssnmhi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3uuuvzlmv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tlqpyimp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3juqlrltl.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xbdvmsup.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aacnthly.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vwdvjyyi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3diubvzfq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3prmmzxyg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ojuqmzbh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vacazqat.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3sieiroqz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ymegdybw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qfwzyecd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3yfevcoma.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3blpwaczv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yqjascdt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lkbxwnob.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dhxnkztn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3kndyegfg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3zruwxhnt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nesuqpia.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xgraelmg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbqsdqlf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sbqbfbaz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3bvucrfno.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uyynapsq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3xsclocrq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3dauopenf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3dtryircg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3oeuikpoo.html


<!-- 参考信息 -->