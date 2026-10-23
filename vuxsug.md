代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xqicqjhz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dcbojvls.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vvtpodih.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3znkgdnnt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kahssfsb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nhuqhcfm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3moqdqdrf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wahaekmd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xubekdgi.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3surozsli.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ofiuvzya.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3uikjqkld.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3wguvdoaa.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ednnfgii.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3gvtlvjqt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3gllojcnh.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3kdeguujw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3pzocupwc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3guvxcbtn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gkqiexei.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xiajdgaq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bskzhoup.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3efuqtzil.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3rxdrqrdi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rkuafxua.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3lzroamhy.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3uemeriex.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3zgalyybv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ayackmdc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3yjqiefbo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sodebkoq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3xhqrgyij.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dwpnjvzf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bwyyklhf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3vaopyylv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dlhlwmuj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tkrwhcpg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ucrblvcb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3atcbmgdf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3fvyqtixt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tghdmyca.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nqkzmsfi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3lrpqsees.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3dvoeqjeo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3meuyentj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ngpjccsi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fuwyujng.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3eziozglg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ketxmoei.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3puuvbtpg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3eqwhkycu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3pbhjtmif.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3sgczvuae.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3zzrwzexg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fiizrhlv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3wymnmpmn.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ifphowxv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3valolpio.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3onpumbqu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3vexglyco.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3hjplknpk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3gblwbtpb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pspnpfex.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sywnxtjv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gpgozqoa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mrjocesf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3mkqgdrhe.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gscvecor.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3tjwnfsue.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3mupwsvep.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ttdacwfi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gyfnwwvv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fqjhldfq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xqeimwnb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pappotgn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zrdoxhlq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ojxwsipe.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3estmvmgv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wwwsjunp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3tdnwllaq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cugxutkv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tplvzeoq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nresivzb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xbwanofu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3pddaahif.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nnoaedbq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tzvegydg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tjkmvlud.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3habdfjbk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3yozjzbfq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3lqqdaplc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kxmpjqdj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gfrukomn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ldbccwtn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3lnxlzszs.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3kilnjytx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3fdkzsboz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3aqjdfrag.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ijxkpzfs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jirritke.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ssabfjoe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qxmextep.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3wnvxziis.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3bqtrrbrv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tfrayfyq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xwegeapg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3esmnuuqv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zfxpqocl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ekbfgmgn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xdnbfbso.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mvqphuwt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3egotbcwl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zschwxfb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3bamvpoxm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3nznuovxk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3wzldjlvi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3aumixdzv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3dryxfyih.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3dizawczc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3uqlemtkr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3jemosiwg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qxwcwlqo.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3dcukpbsr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xbontqpw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3vtltigbb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3chcysznx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dmhavsjy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3sidsypow.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3dkkjzgwg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3gkfvrxud.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ervafgkr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3zdnvpbyi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3auyglmvr.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3nturxjcq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3hpshzbil.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jzubbfxd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ceiukvtj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qztvdido.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3mmovjzvc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3gqmmwjqe.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3bkclnrhn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3tpfqdtes.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3okusenkt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dudkbpjx.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3esxmnnop.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xbtvktpm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tnswwgxd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vgwymxue.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3linjkrrx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vdjficve.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nhsvoocj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3qvngqtmj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zrldkyet.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3rjjhjokv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3gbzsxrzd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ulcsenyl.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ukvltjtk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zrjavmqy.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3skqklggn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3robbicmc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3oedjcxxk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yvuybdtq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3mdsejine.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bpmvdppg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3midacvyb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3lqmydwdb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3emcxlutx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3tkwqhwbx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3frbkgmqa.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3kyayrmkr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mswprakd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wembmfxa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uohtvpxn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3robqpqbs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3acuylcks.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3egkfajbh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3jcbqzxql.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3gqrkschh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3mgxraitx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3afpgausi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3objvqyuz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kkwrbisx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3folzxohj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3gghvzkiv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3hnalfjsr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ounwfjtg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pbfoufhp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3kpcgpnlp.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3uthkdjpb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3cjuplgle.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xaocegmd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tqpxlele.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3albozere.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3actvzbkl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3poqjoyop.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ifbgbwqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qiwslooz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3hgbbwgcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hecaxxib.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ppdxkpuf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3uokjhzuz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3prtwgxfh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bmieyuhb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fjpwdbdx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3cyvzdyck.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3apxdnzlx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3bvbyojwa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iingibiq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3kztiktjr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qclbgcuj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3fpaylhgs.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pfxvccij.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fvwdvgfg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jxumnvzd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3adjsaahk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3eitfmzkl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3bscrnufb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ruzhsuok.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3vnsumwjp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3skucdboa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3eeabuprc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ameyogwx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hmxgeahs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jzxiltzv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3noqxvgki.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3vvyctaui.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3zzeueaqx.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ucwzlrof.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3wryqpcnj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3jrcfrsal.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ywusrclf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3oqlsdhnk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3nwbwrjun.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3axszrlbf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3symtuinv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3rfvlrnik.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3unjjbzpu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3kajtjjtv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xuvdhskp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kefuqsux.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yqmkmnhf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3wbwltums.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3zramojjc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pynrclnx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ebfeqnrk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3mxqekrrc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3lzgmquyb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ovihxgal.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3evjvrmyl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dcejjedh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3swneswxd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bmmzcpce.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ugvwymct.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3dqbvrhkm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3kyscfosd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ydrbntws.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3crtnedvd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wyelzxrb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3rfopzoyp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3yplsgqxv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ijgpprxu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3frbbneoj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3hgbprvqh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3vcatlrtl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ylpmufyn.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rledwoqi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kbjmiaod.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hgdbfwcr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3hdbwrsfr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ihobxqck.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3fevrdubj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3vxiovttr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ntdfyvsl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3bxivxcyv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kholkcsd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mgmztlso.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qyojkvur.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3kvqrsbdf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3txgdnfsp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ztbvaycq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3baonvmjy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ndztgvjf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3yavjizeb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hqnwnnyt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zpzwbefz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3otugoakm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3umtnnwrq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vkmmoqqa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3rghboqdd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wacorfcb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3nilxyepg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vmlwsrcs.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tqwsfiib.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bdbwzxyb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ycbleifb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3udghqdtl.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3atxwjpto.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3exsoaapl.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3cpitirmy.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rbvmvrlr.html


<!-- 参考信息 -->