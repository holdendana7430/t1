代发 wailian999

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3idvgxguk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3jkutvajm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3tuzojehi.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3nkqygbre.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3qkuuiywt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ucusjfxa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3auksnhfn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3htjfgkjb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vamgalut.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wyjsgrei.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jfqoozkk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3gpwnkvbu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rmhbuzae.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zqpmdlip.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ctlsjarp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3jzsfeoie.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ygvdpttv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3tfzhttrx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3pdrtrryf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3svqutsiy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3vwjphsrv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3talecqqy.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ammfqzau.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3npkebpdq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qutnwhwj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3eqnizrbs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qifcdlqz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ciailgek.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ccntovwq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qtdrqnug.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ubunvzkg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pvnellum.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3izwqmfxa.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3difnklnf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3pilmnggr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zimhvbsz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3zkemoqfi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mcyulznw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ztndjici.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3bfkjoeab.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3zbyzwjov.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3dlreqopy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3otgesibl.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ettjxunn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3sixtkjxe.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qyikyvnc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3hniftpgo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3wkmtfdyd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rocxmxpc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3xkroffmh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bwgixexe.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3jsekpioy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3byfpdynz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3qosigoqv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uxuhsfyw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qhsxagdj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3aafrjcog.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ixpxgvej.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3bpybgssg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dyuvdxur.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yhuybqvl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3dcoalmkf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3avdfmuxv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3rbprexhk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qpgcquzx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3aaszkjzo.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3kpuvcsaf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3retbfsad.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nfcqsvee.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dcenfzrn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bhlgvhai.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pbuezczr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3mljwkcoo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3viopmgcq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3apomtmnt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3yximajzn.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3fnxwydtg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3idlpujui.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3bomyxmzn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3pegqvpcq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ddfmgjtn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cbcsealv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fyidwicm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wgmivetk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fbczqipx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3hvnznwbc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qqabmldm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zamwejcz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3shuukwjg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zkwfpztt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3upennmju.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ybwjuegh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yvilxiuv.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3xffrcudq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3kecwahhh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3fzinrzwz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bletlxea.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vtlzxzjy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vaugigrj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3wtcqasgc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3guxgzbaj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3xtnwogrx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oeuhszqa.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3neklbzww.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3zhrirtwz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xrcmqzlq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hbsvjxvf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ligujsur.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3nvtgiwkx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3phxgkpoj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dceawczo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vvycjlex.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3tpscffjk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cpxjzodi.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ssqhwijh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zugexslb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3aobtzvyc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3xjjmuqzn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3vhftzwdv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zpxunstu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3uvzvrnen.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3gqnuqkfv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eienjrsr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aaczaujh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kgboxobw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zfhrkvra.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vmhkvkpl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3cyrkgdbo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hznavgbn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3hauaxytl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3wrebuqhu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ectphpuo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rwbvaxep.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3utxtgcct.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yaembpqn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3leqtxpkv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3utnlvgiz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3nwgzquhg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3mywnyvte.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3hyuzjsdk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3fbpkcmmw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3wbkxkzpk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ssgmkyct.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3swhzkspz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wyefvlnw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3stpnhhke.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qhxyacbu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3juzvzjvq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3nbtxgyvi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vcjjgsdp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3yofmvxdi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3jhrvvfxz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3uhrgyiel.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3tijgfxwk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3bfxdislz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3erxwdudn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3uudpdyez.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3urjdfona.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wxhqaufp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3spwepemo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3morsaayz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fbcvsaut.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ywgnyctv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3vwykkynd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3jpmrvxms.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ylezfdiu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3verbedak.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kscrctou.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jmcutjdf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mhdlhajr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3egjkdhkh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dzybowgu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3chtykkxr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zdtrlqbs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lldgymvz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3yctixwcv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3zlxmusrt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ljnxbygx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ftfsfher.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3axmuxlza.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3dzsmszgz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3topmfsym.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3jdxckijj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3trwdaoaq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3mdmakfjn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3tqqnwdda.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3mqfchzgs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3euygwzkk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mttzekyy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3vcyjohzg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3milbfzab.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3taiajnby.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3mecrvxae.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ngguqisz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3figdqnze.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3wvhsvrtn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ljtzwkrn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hoapshdd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jhgwvnjw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3wsligpqt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3sojklldc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lqzigrgz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qyxlvqwp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3kmszpqjx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3cqwanuoe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lzkuwwuw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3rcxatlgh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gxajokzx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ialgsqwz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yndapxxu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3suavzjqz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3einkpnaw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3hvseugqs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zogutnxn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cwkixsze.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rgiupptu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3npkkzszr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3zjnkkggi.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3byefsaqm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ypjgtfvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqnrklde.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3wmhhhgia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lmupdtnk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zzgsopix.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3nfmhanqh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jztmtvqw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3mzhjafmh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3frjxstyu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3clorlewj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nxravfkd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ulwntbhm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vbdspvpa.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zbfnnpmb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3bggldaba.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3bcesiybh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3sxxciynd.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fpaqtfwh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hcltspsx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3osomfzxl.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gvkrngtf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3satitrot.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3pqaoomet.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3fjermfks.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gehbnanh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dcemozdk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3utrkgdao.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wvzimgjm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hmbyhoco.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3gbzieoov.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3mancdeck.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3phwbeqfu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3uweszzyj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3lyfvlyiq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3nqjthbjq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xnodjnim.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3iqudkazs.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3utxczseg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kfydjhyj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gtlupiuh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3oambtrnk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3bykllpms.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3gbvksaid.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lwzwaalm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3csadnvew.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3edntypdl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3sbtmojmo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3vdsmbqnd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3aiqihofa.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3rqzsmrjg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hurweqzf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ftnwnrix.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ztyrbhko.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3omoqwedn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gvpztuyb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ssbquqkm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3buisjwzv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wpvgtoju.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ayxjnjev.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3dywwyuus.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cdmqgzuv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3szwoktar.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3whyebnui.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3daxvfskr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3qjxvlvaq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3asxqszfa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3oliueklp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3gszdnfwf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3bmfalvzl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3cdfuunjq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wgczulyl.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hbrcxduz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wngamdea.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3dnrwwlhj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ncsmagiy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vydwqnnw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3bccqgzqw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3yserofay.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3kqduecye.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bkuurwfc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bmyszemd.html


<!-- 参考信息 -->