代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3iikmrrfd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3crlaummy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3sjfkenoz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3upvjipav.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3fwfxusst.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cmayjwgx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3bgppklhj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3jjtbkymx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qczurekm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3pklwrrfu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ksjllimu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vhcfmyya.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3npbneuva.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xnnkjguv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3gbzugege.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3otdavmpp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qcudbokb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3oitywdui.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3toizskoc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3omepmscz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ijabuugm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rsidflby.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3aejgmara.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3odgngdvx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3uenfqmnf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lkjbheks.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ynpszvdn.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3awonqkhq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3uxvyigwl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3sikhbymt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wjnampaz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dwgfkvgg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jdycxsuh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uhvhlwbu.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3fprclrly.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xtrrlmdd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mjswtrra.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3itqoaosf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3jmajxxwo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3yrtzsizh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3tadatfpv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3dfkyderb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jqomaknb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3jyghjyfj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3gdvhyzuc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3utavhfky.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3xmoaqkel.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3okxhards.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gvgtyvbe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3nkfftjnj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3bbmhkimf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3cboqzhrw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nnuraqcg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3whavnuur.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ilxphylw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3cgygfmmb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3addbfnmf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xzgfhkel.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3sqtqbgat.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wumqwvnq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ijiijpkn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3sqtfzhgt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3tkbjzbhj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3koostobe.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3jvirrnji.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3iytrxjhm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3karnsdhq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3kpldufqg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3sdlulrle.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tlawgjsm.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3raruqujm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3pgiykyvu.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3fwdqouve.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3lvmauyvx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pvrxeadm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dgvmcenv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vbdgrkgr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qjinrpwn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3rsvupxmu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ktstogpk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wzodjwhp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3gaqiauqg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3zvdffjpx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3kwjxntuv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pdtftukl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3idmiuhtx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gwxulbzm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3uyyjbyxz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3etlljdei.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3taftcmic.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hrrnbbzi.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3reescjlf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3etqrntxp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zukyduna.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kmibweqa.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xrvolzys.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kbkpgqoy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3huvrrfsd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rztydwsi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jqglntct.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3jdxtoren.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zzdfepxw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3hyhhqpxu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ybewfhav.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ttqqiqnn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3thyawaxc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3hregabcj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3agequvzj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3jejpfjwv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3srpkyygk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bacgwgjj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gdirgasi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yobmdoof.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xtlmaotr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3oqkxfhtq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3hprgzbfc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lpatlxgz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3wfpnwqja.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ukznvoxl.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3laftynyt.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3yoboxwgu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3dctafwyg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ziqlkxhh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3vtdvfgxy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3izmhymwz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3mxbqffid.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3psvfsdls.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3uvuindbo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3oejtbzbz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3qigmkfhd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3gtwkekfk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3efxwzvoj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zuajojbe.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ujieojdm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3vgbjdncu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lptxtqsm.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3zayxkvdo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3geldifht.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3eewldrwi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3tcysiila.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nqutnoyq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3omorywed.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3fulaqbfw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3lrkzivpj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3vvchxqrw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3qyhfzcwz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gygcdpwc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xwfncykm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3noiovzxo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3knrkpvbj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3yjwicjdc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3eojqhqwc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3mynskwkh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3iesjnnos.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3rtfsbndo.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vfwgztof.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tlzlysvh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kubqsfxt.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rmsatzvr.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zvaxqdvw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rzcfyslu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hpxkptir.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eridgsdn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3yiiqsjii.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dxhpvdcy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3gvdvzyeg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qkpbqkyc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3uujcsrbx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3fdoohijd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ihuxnvww.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3gcifkxhl.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nikwfmxb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3tlralgzl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ctrybhxk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3xbsgmiyw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3abgdniqn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fzoqjcyt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3wvbufpsc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ypcyfkzg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3glaswmwd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3lqdsatln.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3pmohyisr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3dvsqxmia.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yvxmtpur.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zpphxmzt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nswvpizk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3mpwghpsx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3odstebbd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xhvxiudw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3omawmdfb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3pzfgixgw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3rxqzmavm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lpiztkgz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zfvpwela.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3timgthji.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vglsbgbg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3awgipgat.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3iceskbfb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nbnomths.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3srmnvipf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3lvavesvp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wniyizle.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xugbizam.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3iysjwyhd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gzstioqo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3hmdqlxau.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dfxmljom.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3knljqhfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhebsohj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3tktqbgpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dsmnwkuz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gjombdsd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3srhowvzy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3htjpxlgj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3znqrsrxv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dewcdjac.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3szvjgyky.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rmgrsfdm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3gpvzdfou.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3klbiruyv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ergkkqxo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tqroiwkm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3nvjlmrhs.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hwnfcerf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cxregbhl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mjzzdjme.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ynkaercc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3uqumisok.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3lennoter.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3isxnzfbk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3unggcnrv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ctcrsnyz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ckwmxntj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fwskldjk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tcdxnnef.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ldglzofw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3aetpnizr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3trwyrvny.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3vnywxlvd.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3aduvfokx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3smjedoyx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3pepxnekp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gymzglmm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3litqphfx.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3fnklkbli.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3oxytnmhq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jzxhdktm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3xxjexkyj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3waijueri.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3kooiykbk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qqcdquoz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lherahxa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hpceafvu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3gyfqergl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3skdodqbf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hfuncpnr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3rcsbshgb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vldkjkmg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3erjwkjyi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3waefpzda.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3goewfzmm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kefnvpct.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rziuqqkv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fkmlinub.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ymmetxks.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kerzhtts.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ivrlsvni.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bwidcpqe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ycxnybgv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qnycqdkc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3kjzihkia.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3whlbmpfd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3siwlkpkz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3galwqevk.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3dwvsswgb.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3uhvhybbe.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3eznbsdac.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3unhhbsuj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vtquqhed.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pkscyfmz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3bimxglmg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zggrvkkr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ysvfyyto.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3exripcgf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3bgdxbrsa.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3mkodbghv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bjiaoyez.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3evtjtjii.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tfppzyga.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3btqgndvz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3nnzbsija.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3amxfusph.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hikclwqp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bnblptcl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3kiqxtudn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dosxtjja.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eehdktlh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3knbctovd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uxyrfpsw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ciqtlhdw.html


<!-- 参考信息 -->