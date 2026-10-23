代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3kutorzny.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ndanxgmm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3xyarqcmc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3sezjhcxh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rnvcfaoc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3txgydukj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3jypbpqqv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xfxdhcbs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fddmzefj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3rlvqbnyu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ehqurllh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3iqmbbvpa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ntypptet.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3skmnymvk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ehxppwvq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ypjajlgr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bgiqyzpa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3bnmvndmu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3jpntsyqm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hfnwuwng.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rfhcxsbe.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xkvpsnxx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3pdqixdez.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3unmqriwq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mrqyaxid.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bpjehexu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zpfpmlyy.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3trfoizrx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vwcaxweu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3auiqtmbh.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3tuumuwsg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nhcwrqwb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3dgrlcagv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3psfyueuk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ljrbdsji.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3muuckeof.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3izrocxhx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3anqcujws.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xtnxbote.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3madxzptr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vpusifft.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qwwxxyfq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3rbatlnli.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3hlqrhyjn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mmxxpjzh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3zuwnpqed.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ywdmjlwc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3rupagfqg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3jbacaqkj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3siylowrq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wrlcubsw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3bposukzi.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3qurohmac.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mlppvhcs.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3smvzvkks.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3sywrvvpy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3abwtncdm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3dpolsdia.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wzbdddhm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dhtfdvtd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3colwiakm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rcyhrltl.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3qqigrxlo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3fdkmqwqf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3umarrqdf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3rblslxre.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3brbqrvrh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xwvfebna.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3tiglzzxt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ezeppnaf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3eejwwxww.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wsmgrmof.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3eaxdcmsk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3xspshesc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3khxnlmsu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ghwwtody.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3lbeuipid.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wdlziizy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3yxgofamd.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fbmzbhvo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ibrgdqbq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3buyebmsj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3izphdigz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3aivzieuq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mbiwsckd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3euoecxui.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3hwhugiwm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wtofwidt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3tdyvlghi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3encqadrs.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fvkcrdiz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gjdpkuqc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3uicjpydn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3poszzgrs.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lkledgqh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3mspahwwh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3vsstgpxt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3srkmdcdc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ouahrhtr.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3redtafsj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ynlivyuc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lrbiilbd.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zfmmujde.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dimwlepo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3uiregtnp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ufeiriss.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sosjwbpg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rsmsvzms.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3bsprnguc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eewqxmid.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3mviycabc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dawfwepc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3chacdali.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3pjegzwal.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3mqpfhhbb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3tuiduuxn.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ipvmoxtx.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3aksjxnjc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mfclodti.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qqdbsnjo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3adhtyetq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wsavhdie.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3mhguxyau.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3gkjmfwlj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yetqwsxr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3wbpqmuqt.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3jkvrnabm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zzrcihto.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qsnfuuaq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3equecphn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xtmwaaca.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dwkmkpam.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ccvgxvyb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3vmwaopkl.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wzbmgeuw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3inqrjtlx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3djddvoov.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3jpfursyp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3hoasqmin.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3wpyvmgsd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3mnjkuulk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3vydiperg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hqglyuww.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3msfstyjh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3opjpkfgb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3cgisoeas.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3onhdlxcg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3lxggmyws.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fiabnlxf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3kjxjfjlo.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3xkatmjke.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3zajcgdtm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3fcopxnjy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nklxbwnj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3awrrvjxu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3vivmpzbh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3oykmtbyy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3raznykpb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3tnwokhqs.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3rdwjehfd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3tlsfxmlx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3lwnlnkqb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3izfcmsjh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3sjjjitxi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3unibvlmw.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eoaixiwq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jmsjainm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fxwvyrrm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fzbcirlm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ljddekzw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3anefrelj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3vxeixkrt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3dihjqfmq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3kevgwlpx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ksoxenzj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3eorcylil.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3bpgyjcdv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3lhnxjxol.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3lxjvqxkt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fmvbrmzu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ndebltrr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mzbfwspf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rgzrzdgx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3oihwlyyn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vguupeks.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3cdsutifq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ygazonkx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3cfuphkpn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vwevsnuo.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3qggyarru.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ocywtmfr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3givasuhe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3jvkigofv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3auxdqreo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fmhngyux.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3txakyeme.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ltluqjdp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ugpoiyzk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3yptqhcit.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3sbdhaaon.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3onfxgbvi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxtmyfqb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3rafwgcqd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3utktuhfy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3vnslptxk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3drjgpfjk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3npniashk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ueqaesqo.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3bzagltnt.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ljzpqufz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zhbgsmrn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3agrsqugv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nvxlpmbo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zvlyvqug.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vopkjzwz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tkwmqrjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gcqhgcvv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ryrhjnje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjplbtls.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lwwwxzzl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3yzgfibuv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hmakbtsg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3hkhvppxr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3itynbtqp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3wfzpmayn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3xfrfyuev.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3vnywhuww.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yawaqcgt.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3swthqquo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3aqmqmdyg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tukmwblw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3drsrexcw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vycimidz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oshbhndl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qzzvotmt.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qnknqjpb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3guialngc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ekywtvxk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3nkkjcptu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uymzscaq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uijjukxp.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ungfiyly.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lmzevmpz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nthvrxbl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ahlphxfg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3imeayjow.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3sfxkllul.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3apjgpepy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3huxcsdji.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ktaqpbsp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yhczwxbp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mgynfejd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3nolvrnwx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xwhgkhou.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3urcqhxxq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3zfeualse.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3rrdiclay.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3imfsmimz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ohvoxjbw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3nipcosde.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sxeoefra.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3fzewpbva.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jzaoqrlk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bvvlciyl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3gmkoreok.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fotplnpu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3gawaabzy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ffvfgqqa.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kgxkuqpb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3efbdwkfo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3smolascz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xywsozdp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rkinznrr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jvhkjvfo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jejwvqce.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fbaddzhn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3feojejwh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3fhvjdkgk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3rhmbnzwo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3izrjihvj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3wqyaqeip.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3xnopkool.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3dgwhtjrx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jchtglmc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ozaooywh.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3okwoeotq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jvvwfazh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ygwqutlm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3usunevyv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ugebwsxd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vjzvgbwn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3tntapqtb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3jazzbdml.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fuhthjas.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bihnfwdc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3tqdhzxsb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3eorkcnij.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3qrqsmegg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ylctldef.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kikvumfy.html


<!-- 参考信息 -->