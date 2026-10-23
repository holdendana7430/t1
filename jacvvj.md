代发 wailian999

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ujhzvzpy.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bmvmwdti.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3njvoivmh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3pxqhbsdz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3bavxbrow.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3yzyggper.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3diztdzor.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fmxlnbgt.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vgvztmfd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vuoppxif.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3hzopwepe.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ksgxozoq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vdbvxktl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3kcxycqoh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vbsveaad.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ohqhcaey.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3aqbtacfo.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3mpavhgki.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qtqqzurr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3dgeqdxjf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3zszmczgy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wepkerrh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3xqmibpzy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jjtupkjy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ssazqgux.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3flhntswp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3hvvdhuki.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3jdmvxlry.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xxbrftre.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jrvhocqo.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3kvzlzxcc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3hwdplrdj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zwspspya.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3twrserxd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3okxgtpom.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jssooyoj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3eogfqkep.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3hqydqyzr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3fsqofmff.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3xtmahfrn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3vkobxlyv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3odxuirgw.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bbhpvode.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3tfsyewzm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3txlfsmmy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3nlejoops.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3xvhqvfes.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3snfahymy.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fbotnjzq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3nvugnyhj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ofhnixxf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ufqydkkb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ycvahwfr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rkdgcwur.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3gptifszo.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lzrzdxlt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ubrvcqko.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3cmokvqkm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3kgcnwspg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qrctbtep.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jrkihkjo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ycwouuok.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yecbllbz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jzwrbhuw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3dojhlgrn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3zbpnfqvr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ojidjixu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3bzyzwoex.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3wivimgzy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3frnshkfy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lrdovpqw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3omlheeul.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ccrndiby.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3dubpyfyk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jzaqkweu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tbsqejya.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3wmdpahog.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ocdvhogn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fnlunmka.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zghubidn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3krzmnrox.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3feknycii.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3vahyxsxl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3aqzszenl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xjymplpa.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3vgllmnwg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3twhiypdh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3iywduuei.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ohekfqgj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3egxgtufa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3hkfywfkt.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3bsjnfhas.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3mciuojth.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3jtxksbfx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3yrimluqz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mzwropua.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3mbjqcuec.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3uokzjtcd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ppxzxmmb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3spbzbwjh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fzxgdnmk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3zkppojbj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3mubqluvb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3hoksdjex.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nrodoxgd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3rdksofmz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ckitplzg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3tyspyzbr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zioditzl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3vqczdqwl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ixtybkfw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3noqlohrd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ufhxbzwd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hfapromt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3tpimhwae.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3mdmhaefq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3yqfyurgc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ghnxboqn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3swmtdagt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3smttkkhr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zgynknxt.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3quvlcshj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3evarcyvh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gtswrqrs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wkyemlzq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yzuuxdes.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3obxkprsx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vknanjhy.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3kmerecib.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3bccjlxik.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3exjlpqqg.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3sxcavhuc.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3whutccza.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dvheimol.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mttdzswb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xnfopuji.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3marzmuhy.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3doyzricn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xyrbbedf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3aqqfhqpc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3datrwjad.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3bkjbmnud.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bpifhuht.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3seaxkcgl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3xlvywwhn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3dnftzdyj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3oevwrmxu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3yilkkutn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3nsojxbwj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mjkcdkhn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tdgdnujz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ewonwqhw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3aiugytca.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3aexfdqvs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gjflhurn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3vsrngexl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3xuoiafzp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3vqgomwsr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nbzcdvet.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dcdosuwh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3khufqkff.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gomborqh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3vwjjkftw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ncvhlnbb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xmqdonmf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3jlgxumkm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ikylrwps.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3yzlcbhkr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3esnmnkqh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3khuygkqn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3nmjjeych.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3sxyerzsu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3pyoyxjpl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jppcadut.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ixcohlcf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3wwrulcre.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xuugzzvf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ftdlqcwb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qvhnfikm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rfukejuv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3iztkmwlt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3asudlxsp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qykgoxrn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3peqajlik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bgcmobbn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3nyxsvtzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uyidoqxg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3owrrxsly.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3mhupkgdi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gsqdoxwg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nqykenqe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3biltmiwd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3axoqbnqd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sohapvgx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3upojbgfn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xvumimim.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3tefyjljx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pptzgbnh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3cmgfbksr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ybyjhrbt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qrcgfwhy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rxkwekek.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zurhjxak.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3whzrcfmn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lekudmkf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wpevogwv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3sxqpebxe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3azqbhqvn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fscwszim.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tmdrqsyo.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3adguldpw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3svzunkfv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3vtkfthaz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hjyglbmr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3akgqdyqv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3adquegih.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3sprgsxor.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3mvajciam.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3svwazdkv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fwbocmjw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3fbjzueta.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rviwcedx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vvposdmm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3lgclgaqh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3opqocqyt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3dberzjfz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jjwfupmh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3fclqrsoh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qswurbuj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3nvmqrqwi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jwrtrywi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qteblyyw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3jnsxrrdx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tzhsvasg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3gtebbvnv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ygaxgydw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xymmkjqb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fqsixaxx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3etnhmzyr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wcmcrrru.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tjccrcip.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ypusaofh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3dbribkbo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tjpfaoub.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qnhfpmpu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3lahsrtws.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xwqzpcmc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uhbxhvuk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3wcxnfoqh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3wnbfroet.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3okhrvuvc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3vzliixor.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3yeknzmpl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ooqwkktw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rftiinof.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3oriebthe.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3hmpgwles.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ydmilhmu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dxsocqfg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3golcqzyt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zhzgwqij.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3qootdplp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cgwrpern.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gknkzfaf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3njhcqdnk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3uhghmilh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fzkdwwxv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pdwpdraf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3kofuswqn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yeujxvek.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3wnjwfvvt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xsnrixdi.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3quagaehp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wkbjojls.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lpevrxvc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ktdllpjw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3elzztelt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kvwkkjbo.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pophsqep.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3spltbrsp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mdzayusa.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vilbzftz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oiobbfig.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3imvjvxjd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vakpvyib.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xlzmzbwk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vetwkqge.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yzliifzv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3twlauloo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pigewbad.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qqlyijys.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3rzszwunh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3aqsytbwi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3fdhbhpgp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3wqgrnkkk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rjiujbwi.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3bcdxgwuk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jedrtalx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wlqzbdiz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sedpnihr.html


<!-- 参考信息 -->