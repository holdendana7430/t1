代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2oulfegym.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2uxdegjiw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2xmkqxzcy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2guquteuy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2nocachjl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2gecwfnti.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2gwjqobow.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xuttunzl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2bjdataqd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mocmpeaz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vjbpeojv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ztlfuyto.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ebtrtvjy.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2spmbpkkz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2pnhymbly.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2llvdezhv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2aryobbss.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ztdybznj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2dsvkimfg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vftsuoyv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lztqljbt.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zcyxucyi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2devihiuj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2inqqqchb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vqixxeoq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hgahycmx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bzcgisuk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vodlodfs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2wjvdcsay.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nfsjbgog.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2eoevyccf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2yhbfpbnt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2uxwoslpr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2uixfnrlx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2mwuydfoo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ffvlnoor.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kyrjaubr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2uwuphkqi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ibvrgwlq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2oniahwtj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2urmvnphu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qwstzypf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ichswdsi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2uubssxuk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vhjnnpje.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aivkmyxg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wqcepujk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fhidsykp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2huajapmz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jgzrxcqw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2itnybrkl.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2gmyqdrfa.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2mavqaljf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xpgbrmex.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ygajdkok.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qvfvptfm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2msctqcrz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2unexmqws.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2pkgexiqq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2eqrcglrm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2erzwcfyx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2xopbriqm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wllqsruy.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2tmqelvzz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2evbssmno.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2fbdgiinn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2lrmuiktg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2xeftugjk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2cqpswvtr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tznzonxx.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ppmyumrf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yeusotdc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2utjatcti.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2rtkysixh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2wkyvigyh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2zonnoyju.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ambyvttu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zbrpkknu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2aenvtnwl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2pyuwptvw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kncmdaqu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wdixkiau.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fwedqkge.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2criahkij.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2pqrnozvi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2nlqfjzql.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2skfzjaes.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2cikyjmcy.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ekjrqcse.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2fgjiqjrj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yzcldzxf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2atehzcdl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lzkydpsh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vcachgjj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2msioicxb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zwhwmiia.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ldulegff.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2usprtsbi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2dgxoobwa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2omggjdkq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rxepdqlx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2egwpphxp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2owqktluv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nyzcusoy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2tvrzllrp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2vxlmkqva.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2nbwkilgg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2capocsdo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yjzijquf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2naghfnlm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cuxbmqek.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2uvowpaot.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2oeubnnuj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2lxsmtans.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dqatkxfc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2drwkhdxa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2oxhjbgwo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zjenkoor.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dndpjgjl.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jwtkkpsu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2fveaqjxa.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2plwumnxy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xgoufnzr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jkcyzuai.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2nbnwzzbg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yopdhksf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2deczwean.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vjbfotil.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cgcjganh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2xhctjdjc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2xdzqzerb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2nxatpfek.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2txzbtipw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2mhzncxgm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2sppsavoz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qluhkojb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2omfiseed.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qfejnbry.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2qdmhavjy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2vkfmecgf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jomcthwd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2aukpqgnf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2zhnyfzcp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dvqeoyke.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xqdqiprq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2xewbxujd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mqxenakw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bvgthxnc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ngfkorrz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2soqepnbp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2glhystet.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2jvgjodzi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ugzjfdwt.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ntccipdd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2qggiwkmy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2hxwtobkx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2jwsafeop.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2snvpmwjq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2pdpelstz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hhwseoot.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2yzabuefc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vhfnmcvl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vdfeicpd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2rtlkeupp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gxokilfx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2aglhahyx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2gfcxhlyg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2dffcnvow.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2fpkbhkto.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ilarzdma.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xftvcyxu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2onmokjhm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2htjsuzbl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gfpmrjza.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2zjctzajo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2chbsbecb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2xkptussw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2dczeatrz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2vgzvveky.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lnhkouup.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kyavctvj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sukidqpv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wlpanxzb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gprxrytz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2idfpgyrh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ojvzzqfe.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lznzutvz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2mkezxswv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wvfqzhaz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2zxhfjjym.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jrlmbxed.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2oahyrvne.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rtfcgdpv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kqezycxh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2twsmmkda.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2acidlgox.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2pgzdeisn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cpqhysmp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cefphary.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ssoskfuz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tnlmuxau.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2spgcfzcb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2oeitzndq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2lesgtsky.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2gqnwlrss.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2efyrstnj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ksfvvcjq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bohvodrf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2msiwijnl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2neypnqfp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tosgfaga.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jqfemqcs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2rycrdvpf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2qbbuqvvu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2kfyqrzpa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2qttsiuza.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2orzhwheg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2bzajakec.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2sqsndfmx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ckohripf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2vtmgiord.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hxtrmfaq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zewjswmi.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2twzuelcj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2sjatyujb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cjctzpjv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fsnqfyos.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pzvwjxpz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xmpsgoqr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xuzgtlfp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wygdrlih.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dmsribbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dyvxmdpa.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ggualepi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2netyqpvc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nxgpenpj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2mdfqcucg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2yqzrmwpk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aiexjybu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xoieninh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2pxaupykm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2gbylnkeu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ywobpxin.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mtwrrtpo.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gfxyuhot.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2mwnkwadt.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zblwuwml.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lyatkbqq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kaqcdnru.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fdxcxhbp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ujteruwb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hjnfhlkv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xqchnvhx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zwjivtxv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2bcjbetpp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ttrswqkk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vvydtuao.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jahpssqp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2plfjqhsh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2oaiktiex.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jgzxnhgs.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pxbvfbko.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2whegwtkf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kvfncdzi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2jolvlymc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2nwijoifj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ocnhfzek.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fuaigsmd.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2uykuzrua.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wxyfmqnx.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2knbvemwc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2hpclfbxm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hxseherq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jdvftyij.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hskleryt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2iarhtrhd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qsgutfzj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2eboqyhpc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2fdoviuvt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mxtuucth.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ifmpidsu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cikvvtjf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qblzgmfc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vzunsrwc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2etmyyhuc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2munzclib.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bjmqziqt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2abrpnlcn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mxdvkjdz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2llgqbytk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2cjtnxcca.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jbxuwfqo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ystwkdib.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gaziquxs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2nmrxqhkl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jrwaewvm.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2cgkbvyom.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2bgthemyh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2judhavhp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2fmjroqad.html


<!-- 参考信息 -->