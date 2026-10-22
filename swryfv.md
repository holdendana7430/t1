代发 wailian999

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2gnhuowcy.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2moyygmhs.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2klgzutyq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2dcgtuqsf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ikovqftm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2etllxbzp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2joydfdum.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mvkjqmzx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ezjsudpd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ctljnppg.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ryrckwmv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2euhxswlz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wekhkohd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2llguqaxm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2caxypfux.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2vlxyltac.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2bjkunrwu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2sflcmpzs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2blcskzrp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2tsvsmrpc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lckbatjw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vmmfljap.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ebrmxauq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mwmccxza.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2kfgtongb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2cpmlrder.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2buojbhqv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2myjvvbju.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kyfkiphc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2scztvniq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2dybwsniz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2zwcmexac.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zkyymlzv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ijxkxcon.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lwapzrjh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2udedzgkv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2sbgucwbh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2tjycksxc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2porpxzvc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2tbyxasno.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ixgqxmyr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2gnjeourf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vhlbhsuu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2lcsrinmo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xzxqrnqv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2knolzyco.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2kefstgfu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lvbibjir.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ctolzfty.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2xkyxbwic.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2szcczrmb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cfgjrnsn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wxwwmelg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2clipgrck.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2idfoisnk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzrspzoj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bvwzvxrh.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2bcqmphov.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ioanandi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2rjcfarvh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2abnexeva.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ikwqjcuc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gtzktuba.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pxgbkgub.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2cziybayj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2fijlsvki.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ksvjbsig.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2geojcdvh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2epidlxjv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ogaifwzn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wvfkulgr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wextirgf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2thjuidpk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2auvymjkh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ctiggjsx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tlttfomd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2taluqqri.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2kvbwufpx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yyrnwuvo.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mxmickfe.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2arafulzb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2zfzhiipa.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2sszoozkf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ehdpggxb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2asabghbt.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2vuetuogu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2megsjvwj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zazquohg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kxffsjcg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mjicqzuu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2bmwdtffz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2tjqwjfzk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2vtazmocb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2utrdebht.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wdfcjfmo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2gvfxneou.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2fawzvdkn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kpxysrwh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2chutwdpb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2cnvbmtly.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jrtsmlqp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2wvnibwvw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2xbsiktxt.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2fbtpfxdd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2uzvqxlwd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ahimjhwm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2zbqkciia.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2aiqdalwo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qlrbbkpl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2rhyxjyhh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ftnmjley.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pfnmjyuu.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2cdzghahj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2irewodhn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2yfcmgpkp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2vdjryffh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rlaxahfd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2tmjgbtnh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2rmckwuyg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2eynexhuj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2wbtzxlbf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2kqeezbay.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uxrzcwpv.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ltvlqksv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2sautpfrw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2kasdjhgc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2pvsdudnc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2pywnldty.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2athajgtq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2aksuklvm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2omwwietk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2soutccvb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2atbkruxg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fqqcasay.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rpnjjawh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2etmmecmv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vopmznwo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2yjpexjsi.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pjdiwgkv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2zfudosxk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2cazbryed.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2rnxcoiun.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2zurvefhu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2mgvyaiwm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2zmskzdcm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qzgrfbse.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2lscuhwhm.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2rxuerfqi.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2qdjxyxyp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2awadbori.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2sqmkojmm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cdzywkdj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vrmtefkj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2kdxfcxji.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2sgaspeww.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2xhilitho.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2cojgstrq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xhxmbenk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2aoxnxdvh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bufgoppw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2mhijrsit.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ewwttoce.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2swqaxbfp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2zekvpakt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ffvvuncs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2wnnxfytf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2yringzrv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2klrrjagt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2rvyufxvd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vrzdgejm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2rlseolin.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cmqthoag.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2dbtmopdn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2luauhspl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xxdnoosj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kcajbspu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uvetaexb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uclurhgr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ioxlhmlx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vlfmzyzo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kybwxpbv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lucxheib.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zccaawga.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2odpxgscr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrrzwecu.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ugdkgjtv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwkfysvj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2skoqjwqb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2zdfcpeyg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xtoorghj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hxuztpeh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2psdwmwey.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2akszyhyb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tokhcanu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2fyssmfpd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2idfzehzn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2jovwrxto.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2avrprxpx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2eupdlmpc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fvawdpiw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rghqhefu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ghxxcwig.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ivmyqnwq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ismrzujo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2lxbkwptb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dparhelx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2aursstgz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pibhfaru.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2aoamukwv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lrsunoxg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rfcufraj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ifcgjabc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2aanuulep.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2uggceajp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2iqjnelcm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mchbzidx.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2wbuxpouj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2brybxmuk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wwgsssuj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tyduirew.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2fhsbouus.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2airjdozh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2shpmdhze.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2thrhwndu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2hgfzxzlv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2mbzfgkjy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2stgolblf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2lhzogsap.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zzumqbwn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2xungfbdn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nzwsjlop.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xiwkobdm.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2eonntyfv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bfwkshns.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2dfusczmd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2guxgldgm.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gyaufywb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pnehadnk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mgfbduph.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ftrtwzcw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kguryadx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lmyqimtc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2thgtxaik.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2poadysaf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2osptniqi.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qpkhhssj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2kraitjav.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2nseldggm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2azmahvde.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2fktrsaus.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2syasbtde.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2igciolsu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2pdexvjat.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2faeayhrs.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ubtzpngm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ygpnmklv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2hrzmpipj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ikhdpfeb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ijvtmwgc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2haottiwa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ueocolhu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jfflpcyb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fgilucin.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zxvitqff.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kyxfokbf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2zhdyyiex.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fputmojt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2adjkrcbm.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mvrlzlrp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bmabafox.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wasntixv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nhelzdbo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dvoosbsm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pxpzgenv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ehnbegxp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ljqkkpfm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2nqfhaxug.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2gdvwdimk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zxljydlh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fqozlyev.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vqkpinxg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wqhbofya.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pftrqppq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2eyarlpfl.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2agzxjvyi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2dtvowjqr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zizlbmqy.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yliwtvqa.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2haiupiop.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hdgskgzi.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2uvtlawjs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2yhxcqogh.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2suydezvy.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2sittkblr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2fnqgswec.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2psigjdwh.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2mqloqskw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2nlxgbwtt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mwsghyfl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qgfxdmfe.html


<!-- 参考信息 -->