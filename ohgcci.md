代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2flvzfiou.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2tymjcsfr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ledqrywe.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2xpqjgxzx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2mserldqw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2eeprzhaw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tqgeijbt.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qgumgisg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2fraewpih.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kmlxnaqs.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2qatrvywm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dtuisepf.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2scujjopb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2hleddrae.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2wzrnefss.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2meixesux.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qmhoarrz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ihcsqwpq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ptgrvfhj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rpxzzaqy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kjrgxcib.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bkximemb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mqucltrl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2anlrbbbm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2fmzjtwmz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2vousruel.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2gepudkaq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2cnfmxlgq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2grnlppbx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ipwrkfkb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ahsuwppi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2pqghoozi.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fvvlkstm.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2gxqridgf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2vdbandyt.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hpybphqs.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2teajqckt.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2yuyzwuhb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dpmolner.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2iwdqocsw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xpmjxaqi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2itefrgvd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2kkazzcjg.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mfzjnbpg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxieufxk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2vxkfdyqz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2qznreqsb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cizdgvss.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fifzgmks.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2myhbxzsj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2meqfownj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2hzyqzeso.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ktgywyot.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2uxkllujb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fhdfajrc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2qfdoooqu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nvrynfje.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bxepacsv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pjvpyxbp.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2clibdikv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2bboqpjjf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ozamjxws.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2djcleaoe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zcmbrtvd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2otewlxbd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2uygsqswr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2lnxcultr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qmoepnwu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2frgbkpoh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2zuzdegtu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2zqemleds.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2nlodwbph.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2xdxrjlku.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2tkcxzubo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2comdsbqz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xlsfofsb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2cdhrbuja.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jlsrfnvg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2cyzlmkqp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2zakgunbr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ilzhtioo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2jedhmjzp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2feoguwxy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ydpqgjmr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zhnqoxyl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ebgbxlwr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2akxzbfbt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uhkhxrea.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jiddjihc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2jzztzkxc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2mwhcocjy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2dnnfltlm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ftokxphy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2izwfrztq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2lbgidspi.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2eekoonfv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2swucspwd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vnqzpkij.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2wvuqvgzz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2loigtvvf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2pcpqncqv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dtsywvff.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2hnjwgwtx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2wdhwvhbb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2pxvngcgp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2eiapxmbr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2tzqnvpvl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2uzqumqgl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2gbccepjb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2vzjisouf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kjnpcqex.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2drgeqzwi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ckvxirrd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2imztwllr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ttudkpqo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2zqiriyfk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2qdbnucws.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2yktknjpj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2kitbjjmh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rpycscbi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fcyjczqu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2esusjtkd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ynhslhib.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nnvvtwvq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2giuzjjhn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iditjbud.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjzvyohy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2namnybyi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dgyuafzk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2hkqwyxet.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2cqkpfqvf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2kadyhltn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wkzwgdxl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ckjjqsdf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2kimzemrq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ahvmdbva.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2dtckmrfy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2vcpjplez.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ftjqfubi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sbbmawog.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2cexnyxpf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2qyaeipra.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tjxrsjxy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2yiztnpno.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2oviwwxwi.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2qxfeskab.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jtvuuwnv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2xyrzpunh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2grruvagg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dywihcgu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2nvsywoqv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2arxkrdvk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2csdchrxy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2jeehfpdx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hhevhnjn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2jxsvcvcu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2zamwkqeq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ojbdqfwc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2voavhpat.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2axaumwss.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2erocpwtm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yoeeeetw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wuvycnkx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2imuiqswm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jrgtfoih.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2szvgeonv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ynnuklkc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dpqkerbq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wnrbanfe.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kvgesezr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2beupdwbk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2yuqcsjmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lpjcrgee.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2fgbsotwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdrlbfxh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2awsexztf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2qctdmjdi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2rhabhemx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tuwygadh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ikamxnap.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2zjmaftgd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ekwrodxq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2bvyquxpq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bhelcyor.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fggvnwwy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fxtqxvym.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2drthsuow.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2taooybgn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ztqguzhm.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hcwqprog.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lfmfvaqh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rrmbadrk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2eedsrvnt.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hxiiffvn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2hzekmpww.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pvhcbqfb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gftilshp.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iqdhwygj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rpithtxx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2nsndcwpo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ccgykqcn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2gdmedbdq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2nemawaxe.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2sqzvaxyr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2suzmzkrn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2elvglvwn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2evudadoe.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zprgakmg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2yfvlzxnk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jtvshwlx.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2didbgzyc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2wkmqgtyt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2odshglrq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2lnxfxvzg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bbwnvlal.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2guigooez.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ndexudsd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2xhfgvcay.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2wjsndidh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kahayghg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2noiexjqe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sygmjvol.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2nyybixei.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ijgkewdv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hoqsygel.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2goupndxm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2daxpblip.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pluvpnsm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ickzxdnm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hygienmr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2veguiocf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gvfpvuxv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yhyskagq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zqzntuuz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2iwlrfxah.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pkfkfcij.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ynwqbojw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2iqbsuqcs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2gyadrrcg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2govvyqml.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2kcyaieme.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wxhirigk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mgndrzyu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gcffrteu.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2vhchglyg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2avmqtqkg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jcypdwdl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2zqepuyfm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ptyayres.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rhwybmxx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bocxkmst.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lfnqqyyb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zzcmrtju.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2srcveetz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2zikagkqb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2yzvbudgp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2bgieduvi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2eecoxdii.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2iljyiawg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pejjisuw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2etdnaiva.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2scuqhqwr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pvdjnros.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lqhcdvtt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ydehbswx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2hgfbyots.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2gowisele.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2obzgmdfy.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2klzmkpue.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sbakefet.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zfzosoqo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vhdcxgof.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nmkpzodn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ssraklwk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2kivqpuzh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oqouiwmd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2sbtoramm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xvnszopt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dounilov.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ooujxxog.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2pnkgjmdq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2avkystyg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2gwvoctvx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gtfcjmul.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2pftyiygw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2qxncvgyo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zccvqexx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2imzwkivq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2asecejhm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2fhrisjov.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2sxcauyum.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hecxetkg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2xbwhanyc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2tdcpzrek.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2fveqhxuw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2egurgkez.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2lbsugzkc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2knxwwtfx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2dfjjwbed.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2yigvlnwf.html


<!-- 参考信息 -->