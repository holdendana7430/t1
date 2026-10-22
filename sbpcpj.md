代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2slqfdyyb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2njdifxtk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vqvrbacz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fvftpqut.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2raxtkfoz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mfjhgyri.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wklhytzj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rdkesfbh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2fcfsdolh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qkgzwihu.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2epcbudff.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2jkobeoma.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2gdaeupog.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2pqnlewem.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nvwwpbzg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2aarmztkm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ozlmwbwh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ahchtlfv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2bffwruww.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2iosmbqth.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kyaydjez.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ivbbkqvn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2coewvoal.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2tgugrcbs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2dkbbtyve.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2nqyajvbx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2shixpdgj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2yevolnix.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aogmmwms.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2limdnjtr.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2mxbbebec.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zxsavbti.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2jasaxqyq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2pfnvkqxs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ipldwmrs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2mbnqizlz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ncerezsr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uthnvali.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2jnxyomow.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2gwvlhwos.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rgcbeuyd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ynynacuf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uqchpxos.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jjvngfpx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2grfkouuf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ayccglvb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2memfdxss.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2bbumrfsf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ikeemotp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2sgnvhamc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eusvpudh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2wwjwsrfm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ulynarzn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ruecvoyt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bytrymyu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2cdzexkym.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2prvbivga.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2dtdplzzy.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2grxryefr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ixzwlqce.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2opnqaeaz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oxxiwgyt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2dksppwrg.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lmjhnzfn.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2uljlawke.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2clmvtcpr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ujpabehl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2uppkpioc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2eziqgkpn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2inoektaj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2sxjynxaw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qfbbqdzi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2wicqzfdl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xahcxqaz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zrrghzmv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2yqrygvyf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qgasvfca.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tugccszy.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2klxyzyhd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vksorvvr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rufbxsik.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2asuplwnc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hgijelhy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2idhbrmvh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2llllpqbd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ugkyonkh.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2gucwkafg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ommvwyln.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tfebrbje.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ekikvrrt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2untwtmau.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2rlmhonfq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vhoknzhs.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2sbrosice.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2efqohncb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2auyzxcbi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uuwxtuzc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vrwgyehd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ydqpzoht.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rbswdwun.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nlmtbwos.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2fcdkijgi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fopmnqoy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2utulqmpq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2utewrayk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2hsomxqqo.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2kzlbflcc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ydohdsup.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2orfncjku.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2hlztoyvb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2axeepuxa.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2jcxxjeoy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2fdotwumu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ywmmuhyy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2yfzafqbl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2scwmvups.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tsdnsxic.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2uxnqxcqf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2bcswdjvt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tucldbua.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2amoivznn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2fkjswehw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2nocnidiy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2haengqbc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2yiukwwct.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2xpjzrrlr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2bfnzgbfm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2nhwiqkhu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2xavxyyqu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2kxlbhncu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2fztossxg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wzajilxr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2sunflodw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2rpztawhq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2sctczyjh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ztxzowye.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2igdeaypu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2hjefnyyg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2tjjgguou.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2jrwmzgtb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2puftwilu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xwobzmvn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ogtfttpg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fqybfyih.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vqgtxefd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mzvygyvu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vtlasyob.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ldlsjvsn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2faegwydz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2qbftpoqv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2swpjoovh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2fwyckrjz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ibuffnwu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2obhlohzh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2jqqewckl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2gcjyxfkf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2hsiahgsp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2hwjtnnzb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2niddavjm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yaomqhss.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qbjmywwl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2grtzttty.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2eptxyjmz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2jpjeqxqz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2gwfiuwqq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2necoxvgw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tsufrjmh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oqtrnurw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2mbfwpsok.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sckaliik.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2eiokniea.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2sgpihten.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2oyywedyo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2jihrbura.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vgggswxp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2wbribcpv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2woqgxlqt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rjtlkcpp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2vvyfpicr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ebtlwxih.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2gixrsuhw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zfbodyfj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2derjzbaf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wrmfuifv.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ujjnzqai.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gdhgfyon.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2blwovquc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dnjkvolq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qcxamtyv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ossfbrtv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mykglnjp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bvvudauk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhgqqlfr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2cagybgka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldlibqcr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zqzdbjcf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2penwvhrt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2guxpojbl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cglcsdim.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2usivdmcq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2vjbnqwww.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2emgucpxf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2kzjfypkv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pqechjnm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2puboqjbe.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jmrfsmrc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aobrrprh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sysvshku.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dlmxnidj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zeicpvpr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xaqvwoxq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bxwnurik.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2wvnjofxs.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2cpneoofp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2jphispvz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2twwlyfbx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zedlitjh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aziipkfn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bavplddi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yvumsvug.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ahkvxmon.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2sfjbwghx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2yvahorak.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kdrptche.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2zyavpanh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2hqzvcvpb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bopfrigs.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jngzcsfu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2zcvmwqgh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jbjqqkyx.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dcjzrsvh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ejaeecwd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2okndvoxq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2milhijue.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2atakwifg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2qhowsacl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uvkoskkj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ofexjwnq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2axtvrnch.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bdgribkc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2otstuqoi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lpynnraw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mucsxksc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dudhrrdy.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2coxsntfo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eetshsdj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2csvggutl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cklvccpp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xkumurqp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2clkrlbbp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ggessaaf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2elzriptq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2kaavqurn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uaujhoey.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jguowxwm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2owcjxosp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2kujvlcjh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ryaqjegh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2mjmdmlei.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2fiuzohdz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ergszsrb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vfvelhfo.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jtaguoaj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cozjubia.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2jklwwmqm.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jsylzeka.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zqviaspw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2jybtyegk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2djlpqnvy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2jshqsyxo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ksgumbzl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2shschvyp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vehxhatv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2mibbnary.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2aztdcdcb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2upwbreda.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2aujystyj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vddkyrpu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2yktodvsr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jjnrtwah.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mlvrzzgn.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2uqmwytly.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2govmbzcp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kbcdqxsa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2dxnpuexa.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2hqtuzzaw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jmgeltcy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2knmwnahc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2susafrbf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cwlgxtcj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gmysgabq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2glearafk.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2mdngkqni.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2raarrbfo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2pegjyoxw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xhkdsqtw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2nialiine.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2phpnfsib.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2unfdlpxk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2mztihwde.html


<!-- 参考信息 -->