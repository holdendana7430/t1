代发 wailian999

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dbriovzx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ptumbnkr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2oixoqnpo.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iyhesjoh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2mxayozye.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pvlqgats.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2iotkezty.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2zjpvxsbl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qvnwigqh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mztpwisr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nbklnwos.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2qgisurpz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qzkgonzm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bxxenbcz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2bjubdado.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2dphlbtaw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2hephlykt.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zhuspwyj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ciwlgymp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2esmoyifd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2txvafjif.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2egugzszs.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2guxtujyw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2codlqnaj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2flypjnyx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yfclozyb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2jugjqaau.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2netevtyg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2aqvcwkto.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nfqentur.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ipdptlnn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ughrqvzl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zbabgfrp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ilcmppju.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2dwtmjbxj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bavupxhr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2qquhelsd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xfmnjbdx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2dncihayn.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2uvqmwmzq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2dugfjldm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xzbfaaay.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ppchlkhd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2eckqybpd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wifqulsp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mesyvqeo.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ksutwabu.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rtcgzbio.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cnbqziwc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ssnmvauk.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bsmvouby.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ybckkddu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2rxihfbtf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2wmocspau.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2cwqwvaoq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2onhuayxc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zlyhtjoi.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yledxevu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2mplsvlwh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xvbwrwfr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2tqqqoorj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2aaiznnra.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2foxlnulu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2hpdxfpbr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ybiiewyi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mjowmrtx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2bcravxos.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2uokofwym.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2udfqhvem.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2varlpuyb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mlqnpwym.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2sroedhdc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2tpmlrgfx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ysecdajl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2rmlztqmz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2pkoqryom.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2svyhjhji.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2wvkqvnem.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2owkpzjov.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ldkffiwy.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2szsvszov.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2actpnssq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2fjbbwqda.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2fddaclvp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2agqztmyx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2yscjnwkr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2awgxnidf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2cyfexran.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aozkysqz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2labebdyu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2rqzrjhaa.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tqmivkzt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2flubojay.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2mnszhzas.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2soveznaj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yqfczocr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gftprcud.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vuwaoxdo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2idwglztv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2dlvzukob.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2mrnygeqd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2jrwgwfkt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2feguaqhv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2tbudybnq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2montfgdx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dtzbcevj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2sjtsraea.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2sviipkij.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2zpvmstxs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2obzznyyp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mvxhfcvy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qflivrki.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2sjltbrjc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vmhtawfu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nalzbzkh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wvdtodhy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wmkvxyio.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ghulqsbr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2vnwasfgd.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ejvokrzz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hfmzovcu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2cmjjbqiz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2azirkgoa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cqlowcun.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mzgvwqtu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mqujtyko.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2wanjkvvb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2vzmkvtnz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2rpixgocy.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2vyphefyf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fwwayvtw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2drvymhjj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mejsmjmi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2swnlwkuh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xcdlsuiz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gqypozbc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2aabbzkwc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ejibfusi.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2hneerfww.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2rmtvaptx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2kfzcofio.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2hpkcfpxs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2eucvgwms.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2awhacqhy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2rkipesui.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2caymfhag.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2grijrfid.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fcsnscjf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2uvpovvfr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zlyjjhqr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2pttjowha.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2yhlyifaz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jwbsdjzl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2tpqiibio.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wtmztzwn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2fvhbylns.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ioftswgs.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2cpgajzni.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2iywwgmnt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2fxpntxrz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2exufadch.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2rimwyddx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2xqamskxh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2hfoxpmjx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jxyxrqyb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2cfnahxwg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2hhhkcttf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mjnfyurt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zxtadbhn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hufndqkp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2orxqsowb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vszubdgo.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fonbklok.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bzifvwfu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nlalnxbl.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2bbdsxmjf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fikpygoa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2tqhjmdum.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2dlqlaoig.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2xafzpwhi.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2avqtuyyv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2unqxekzs.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2adbfznqv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lrsqouoz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2fhmtplge.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2whrtrfhf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2exylppti.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ntvdfuyd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yaozdeyy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2wmasubum.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hajemalx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2motjncrs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2rkajnhla.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2oryxoxff.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2gfgvbmuo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2iwfgynin.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2fogtoymq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2obyepmed.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ubpkhson.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2sxornvee.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2wyqumadk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2fqdudvmn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2mufrgzow.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zhuzzvfw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qhkioqpw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2xhssqvpe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2gpqgkhcn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xlmaskce.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2rcjvztav.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2dnkokrzh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jntpgvdz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vbuggzny.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fgtpiuqr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2thwpwinv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ermxetfa.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2buiojwza.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2adxthxry.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xgxlzijq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tivslier.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lpzqtcyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2juinezee.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2rpunqyzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfbvrphm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yoolsiir.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2scskexdo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mypbjcps.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2embuxzwp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2miqteqsv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2mkzeeyqb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2zekdxwgl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2nvtjqecu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pwbkybfe.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rvrfxgti.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2pwphpayk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zehdylbg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rhxndrbc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vyrzvzpm.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ixzirhja.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2cdlphdst.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2raguqkog.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gxczubth.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dcgnsguz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2lwwylhui.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lqbhjowl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ibybnusv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2acutiamr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pyepzuyj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2yofmnrke.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2uscaozxz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2nobyidak.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2yvccetpy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vjzsjbwl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2euqqcvnf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2gjkfsord.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xsjkxoca.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qcydublk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2feflvqcw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2euibxhjg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2enjtyjpc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ebosgtfa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2qyuufile.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2bdttkqsf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2absyvwwr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mlxhrlrd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2myxzbepe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2owgctfhi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iaafmwgr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2oyqrefpp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2qanmpmoh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hzzsjvbw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ifbpprkf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zwaowxtw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jqogfcre.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tuztncrj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sormerjg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2trnltysf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lhoqzdyh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rkosifak.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ijdfibvv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nsgtulrs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2bqubuzyx.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nmlvaugi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ajzbschb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ejrbpipz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2qovepson.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2qpgqwqpg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2xxndskfk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vrxwqlrg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2trkeebpx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mokrmtzz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2agziuuam.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2eomghegl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2riraawix.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jojkogmv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bmmlvdig.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2bmjqadiu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vlqbvyfv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2xriusrsp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sgxjwboj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kzitaqkg.html


<!-- 参考信息 -->