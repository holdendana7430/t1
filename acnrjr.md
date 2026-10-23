代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3leupzaek.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3opinekhl.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3eghhgphq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3zhjrtrjx.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dfienqpc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ypmuptlv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3epiuhkqa.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3gkxamfru.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3jlgckzqv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3afyuvmec.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xbxitlhb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3dcdilwsk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3khtonrof.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xzfguuct.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ylqlpigh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kkvpehhf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3bzpkukaj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ztubcztx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3mevsvklv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3fnfjshba.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kiuescio.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ntmxxmgs.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3licuzvxu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3bxnvncjq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3hajtkldv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ajeowggu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tpwegxbh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zhsumxoz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3glcqagcu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3dtoqpihz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3fikdgsoz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3qfrlxzcy.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3skhwpcut.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3wdrgamvs.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mlufxrry.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3dpmbndhc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3krxiryea.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hjhdpoyg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3chsxokff.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rvyqlvsm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3qeqzbtcp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3uhpiysut.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mvafjspn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3cgsfgtyv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kydhchhv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bjlnutms.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3zgsfurvz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3swtwclvg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3mmphzqvo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3hqevaevg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3cczascdg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mcoscfxx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3lspgeult.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3esmxfuqg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rbhtvztd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3hhdmtdmh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3mytccrgb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3expwpugv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yuzocrve.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3seiwvqeg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mbmksfkf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zhgeeais.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sqrnycky.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fqorzwhp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3celodnwg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3eqhdkhjn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tzzpofwi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ijrbxnxf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tfwxyjop.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3insjyzya.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3poytfvzq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dxdfcigl.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3iskvrndc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3bujlklik.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wwzheyzw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3bmfgtpnj.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nampxrps.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3zgjqyokj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3anptzpyj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qgtzebrr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sgejcnvq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bxvjdphs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3fekwzqla.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3zrnikugc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3bzvsrvuv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3tooyvtlb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3abppiusf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3arqckpvf.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ynswieao.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lswsfxuh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iaomwega.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zivvnavb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tpiifljm.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3niemtmfu.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3osdkypsj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3hpkjwcur.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3dnnwpuym.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3utzuklue.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mujkqmmr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ohsayker.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3epxxgqdq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jhwzhnzo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3zfjnbdmg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mgfmwwso.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3gjwjckrt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ffrrbybe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3iyazdvhi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3gcwlbubg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ymqdufxb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3spyxfbzq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ucleqdlj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3srgijxua.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3pckrhbhd.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ahooownr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jurcystf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3tfkxzpmo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fxldgdzk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3sjgyavrz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3rjjwiiio.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3islzdoks.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3xkoaxczc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3vdiktaed.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3srgegtos.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3qwowzmzj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pirlgcpc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gfjzuqld.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jtmnsicc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mwkoarvz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uccevwpu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qyhtoecl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eiulgeuo.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3smbnavsb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3aziinshc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3vscfpyoo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3exvzqrfy.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3wbbtimdz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ctqreugf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3eremxurr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3pyjqxsuk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tvkqhmkv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3szgqukvc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ogsnxjub.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3rtrsirod.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qaygxxad.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ilybtkmx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3fxotpmiz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hidaewhh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3tjhfmtov.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3igwyewzj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3bvxppeqn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kpeqfdmn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yqwmpmyo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kgpuwvxa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lcjtaffk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xaidqkvp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3gaukuely.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3aifnqitx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3vneqezgy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3dwpehaav.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3owxkzuci.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3sphgvoug.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aiiathbm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3eluwomqw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ciqfdmco.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3nkhcvdfe.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3njkncfme.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3tokkhhxq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jmedadip.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3brbimydl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mjfaidcb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3exyyjdgc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yoxxzgsu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3alyyimxl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3zbhbsqpc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wkuehcce.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3btyzwyvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tptaktij.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3gxdoupgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xwfhoaxr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jaoktgli.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3yqnrmynu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ihlmymsq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vgxlabgv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rtxdrrtk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3gvtaebaq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3dvwbjdgk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3pwriwjyc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3frettvmj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qaifqtol.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3uvupkjcd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qycldgdn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cqeennjf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pedylxjr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qijvciyu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eavlsgaq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3guwmrhbg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yfqfrogg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ijqsnlht.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3uuxswjwz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lflcxvae.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ykesyryb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hlbkbqdn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yyrluaje.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3utabptpp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3azzdqjox.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3dngvfplb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3hryguzsu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3pecwxrdj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3qykaaayt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3lnreriju.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tizipcud.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xxzhbwbl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ceauirjv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3odovgywx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3faypmrup.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3sieisbsx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3krcjksta.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3migwlatq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sektdeqq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bjhxisio.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sqsusuom.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3bypovpyd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3qwpdlchq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rfiozyrn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3dhrztdwa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yliubllr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3vszegiem.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ziuhbubp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bwqwtjsz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wlwayoot.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ipillfzi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ponyzjer.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oldlibir.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tnxasumw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3pblptivh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kfsdelaf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3uwbqnvbj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yicyhxaf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3hibrweot.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3shippzrj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3vqobdnao.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3coqxvotj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3tbncmpae.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3tocjkvul.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ixpviuzl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3eqwalyhn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ebnxbopp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3iujqsyqf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3socxrdrk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mdfdbpmc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ybuiwtge.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3nnwgoows.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dwfseywx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ftevxaks.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aqtbzsda.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ykfsltyt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3dcnxhklw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3oggthsyr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fmqcxhbg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3deelsosm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3gbivzovk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cfnfsewx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xykvuxga.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jfzchczy.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tympqicv.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fhfzyqwc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3spgyfsty.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hjzcsnal.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3okehcgdi.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3arvoqcmp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lgtacujk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rycghvfx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mngsvnjv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3geslzvpf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ypriuqha.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3iajbzzhv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rndwsicj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fyiigatg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3uobuznim.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3efbznehb.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3vaacwggm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fsrclkul.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3btlexuud.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3fpuibklu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3vuelyqtt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fnhopmfb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3feiiezbu.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3xqoodxuo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3msjaezfo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqjlrihm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdytzzwi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpyomsde.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qeitcdnb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lexrbhzc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3nofuibyq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjklmvig.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ztptotoh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3optahbnt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pusqeims.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3knkzyixh.html


<!-- 参考信息 -->