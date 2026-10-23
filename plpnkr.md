代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nlrvqekt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jjngculd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ztdiplqg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3plfcyoki.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ykcdishg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3acspftaf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3sojguqew.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3yhmgtnws.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3kdltjrad.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ydemzutt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3utwzmusi.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ppomdtml.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ksuupedd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3jjabyiog.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tclobpui.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xdksbxqv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cfxalxqp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qkangceh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3tqrfjnul.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3njjpqnno.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wregzlbs.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3csyagost.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zxzzybor.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3fwppkigq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3zetciolp.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3vjbwvtfi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oujwbaxy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3zfefwyez.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3jhfpbkkq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hqjjvetz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3dkhoijzl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3dyvhrooi.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ssjglyvb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3wvfquqwj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ulziljrj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3pyxtpabk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ifhqeair.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3smhbnxfq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3tpavdnuu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3skzklkrs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3bvzxdyns.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cpvxlkbu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kiqgnbld.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xvtxeocp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3vhzkjiyw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3pzohheni.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3kbfrustc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3rkxhxrfb.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3kkhdittf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vlktnnit.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3soasqtsj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3vxekpjgb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3qjndvenk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3xdxzlqkl.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xdxkwfuv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3oboqmoyj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xjnbtrtt.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3yakewfpw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3lzhbupdh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hlvgmoyb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qntnwvcm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3viutjsxw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3vkemytzl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rhwkiwix.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ukrpvsiu.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3nbucqbkq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3hwswiheh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3nkrwxior.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3actuxauq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ytzqofyz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wrosexbf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dkufyunp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3assktvvn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3pdhyrcxj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3msdjwsml.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3rpjardwc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3vedsxlyu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3efngwwyn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jcrjjobb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wnbfouwu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yuwfllmp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3zrfbmtor.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xyrcuyso.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3exorthcp.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3etydeyso.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vthppwfg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3agiaxwrm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3laoqifhy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jiiwoctn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3jiscougc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3kzzbsaii.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3bzchyiql.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gtzfeujo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3nygmlsdb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lbhqsyxd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pxwbjdkv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3oeatcqzk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ywxynsqi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3jxdhdstr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3exfhhszo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ltcqhlhl.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xctnyuwc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wwquojgk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3exdlbfqi.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3pzgmtyab.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wixqplut.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qppzbkvz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3sbkxrimz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qpufzamj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3gmyilhwb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ytbabzda.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3uookurrr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3cightqej.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3nlvtlqpw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ugilblip.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3dfdponxm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3khlvcrzt.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3errwwkpg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3cuoriekf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rbnmvyap.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3eqqkcnsa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bdghckhe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3uggizxll.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3nfbdfuxs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3iqekfxva.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wupvphrf.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3aveecici.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3yrgcmxdf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3pphewxdq.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vnsecfns.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nmhcdwbx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yzoptfyd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3lkvlslan.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dfwgcwvn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3dzllojms.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vbpyjseb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3yyoswvzn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3gzcyshnx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3aojbghko.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wzbyajlv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3cuoigtvm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3surtrmqd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lnukpvfu.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3edsgwfjk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eozeutjl.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sgijxkya.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kojzjlld.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3izkfqxcr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mrqlpfag.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3vpuslzsw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bbbyywnf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3yqubottn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nuiozvij.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wyphhydh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rqyimvba.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3stxismsj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3fkmdcgnu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3dlijvfsr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3avtspxwg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dodtgusq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xgjnkrzb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3kejwjhtn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xttzmvsc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3edodsnmz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3kvjzckuy.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3bnybtmkw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3svzqiwtj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ebudurqu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gnuypiwp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3edgtjmkq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3uuepfvjt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3hxwrutkg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3tkmhgaju.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3txpfgaxf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3dpzxhfng.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3gwysnjlp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3rapwolxp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3lwbdixkd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vxpjxwxy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tkgxsjhm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ifhcopsv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3opubhsmb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3usdoykmp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3maliqlsm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3moahvgtp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3eahhegiw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3twlveqfy.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3aitcjewm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3iimgqkmi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3emauimfk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3oqesplsi.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xwbvoqak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hviwppop.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3xyremmsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3neuckpmq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rpgepeps.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3yympjbmy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oqrqnarv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jzazgqmy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jznygeru.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3fkwjaajs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3uahzgemt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3jzumphlv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3giieuaym.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3uguekxru.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wdkysino.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fopitbts.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xpojzvcm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3axtxxgae.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xyvnsygy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ciwsykmt.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vwibntte.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ftaodvwd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3deibpepf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3cjeyjwnr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qdroceef.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cpprthmd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lkljieoi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3panayjji.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xylyfsfc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3txvpfyul.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3osddbyat.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3latbbjcp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rqoqpdxp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3udgllqao.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3egheqezh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3iruyqapc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ufbimkav.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3romlzitz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rnhrwylc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gyuufekt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qfcesqxv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lgjpibov.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3hurywxbn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wvrlsssb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uiyhqchp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fvmxgiah.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3blfpzpgl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3byankvub.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jrtqtmnr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3kewbruoq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qgknkuxu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3trwxwzap.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ducyfwbs.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3psnyqqpy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qztkmeub.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3husneamd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hjydvxwy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jgkqrrji.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yhtwgocs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3wriyxcym.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ikeihkxo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3adigsaen.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xhbxrdbk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3grayaqlc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3cswbxkzz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3imgiihsy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3rlinenpg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xsimhinl.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3htsvkipv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3pfxbjzre.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wpiivwne.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zxaoidmm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3bsotchzw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3kxeikmwi.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ksvjsnag.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zycemfrd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3obeaqbos.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vcjcyqrf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3nsoagfpa.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gdfefcst.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rmefmdva.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kxtukjrt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3fzeifmxm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3clcudyee.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qsrrtdri.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3stosdyxy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zyhylbmk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3whotdpog.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qrmtdnyi.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fmlkhggm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nwqnipaw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rvhaaffv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3inzcgxfr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3zlgrbtzz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3moaateyv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3shuaggxa.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3thseaatb.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gpfherzy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kmnxlizd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3tsrdmjyu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3loqmxkkv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rynukekt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hjgzdsjx.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tcoctfue.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nsgbstxh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3bxmdzlka.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fkvdwler.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lpjeppsl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3vfhptfoo.html


<!-- 参考信息 -->