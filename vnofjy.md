代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wkvubafb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3eaqmqffr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ffrtcsuf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ozdamrmo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3vrgfpwue.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jaqzdfpy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3bphjogum.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3xllbucbp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3gwpelnty.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3gngbrjti.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ziomdnhh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wdfyqmwt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zcsrvpvx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3hhbywixz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3rmlxewlf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3egnhcnna.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3uimnaxgy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cdnjqvhy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3dsplxuix.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ibcgekno.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3raccosan.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3psxadzki.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rcswmhjy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3beidkumo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cuvzjgsb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fxyxwusw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bjrdbcay.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3wcepkcqa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3kayzetcu.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ewrphrrx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fcjvvhpt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3voysoyfq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3inzhvuah.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3xifbvvad.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3edakyeou.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wqdkluqi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vmwaumir.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vnjosyfs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ruuztozc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3iaxotuce.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ngcsqmjj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yicjfqnx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ienajakp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fwdexsad.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ompcwblw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3eqeqsqtz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3owgwrrur.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ygqtxxty.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3bteroedm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fujezfed.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3jwimycuv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3uaemeyan.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3vtjivaak.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3virjyuxg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lbypfcdn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cmxicmhk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gdnvdubi.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3oaxgmxkj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3chducgmt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3xlfvauim.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ugueqmjy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3iqocmbeh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xpmamxoj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3tuyhpmys.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3txemtmcg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3joyrofne.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3marvxolj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3zmursmsj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pmctatnf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nmianbqa.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3tqueabvh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ngznjokl.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jvvzdten.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3pjoqknym.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ipggqwym.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3qzbtxiob.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fxlzphbe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3chfsetmw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3hkzrhefs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3hrlokwvl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gedndpib.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3asepytoj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qcdhwahz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3unmolosv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3vxvknbao.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3oxekwuki.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3izbhlzle.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3qgskwcxx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3nfmuntgj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3skdvhffp.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3mjkdcwyt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ngroodxd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3tstahxqm.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3pewzjyxo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3gwvwbtyo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3zqlwnoqq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3stzyzlak.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3daxgwwfo.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3aspmrivg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qnegycpf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kicbslhv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pdxpzllp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3jkauhyyr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bnzqkdyn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fplcafcy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ckyphydw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3epkcberw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qiwlneqa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3euteznla.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zbwfnrfh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hducjxvl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wfsatemr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3gcanmjpn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3rruaelcn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zbheqsrd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xcoaxoen.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hhacjoym.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3rlfbuuaq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqzvjbtc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3agpncozc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pkvmwnaz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ftucspng.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3imtgooqb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wgdxthfl.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3xouadrce.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3oghkvzap.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xitcntvp.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jjflkqar.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3oontfljk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3kqnozmqy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3dewdmhiy.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3vzssnguh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3vknnaohz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3motnklwp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nmzwgypn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lhhsnmxf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3drtvengy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kwcfrjnk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3kggfznzr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3itxkfsqn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ayuygkas.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3zjwypnyc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vpwgkcmx.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qcsprlbe.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nkkwyopb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3anfjjaxd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qbhcthkl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fzgevxsi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wggbqnbr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3lzfcpfkg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3tmebydpc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3iyncejbq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ijbxekov.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3bsoecsyc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3kqefpwmo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3czbbqoqf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kgvrgprt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3xnnjxjfc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3kdosgzpp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ibemtgha.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ikebudok.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ykqjnqsi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qmqvldke.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3xcstcerl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3uomomzfr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3hddtlgxq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ormiefyr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ggylkipr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3dhnwjfan.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3wtlkbfap.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3uqbtojdy.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3citncfaw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3bavixlgf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3sxczmywv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ljegqdcn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3xbbbpasz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3nltwxakn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3gzwpivog.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3pnjjxazw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3swzohwtz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3bloadkdw.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rclrjcph.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fntmwvtf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pcjvehfe.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ohfsijty.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gkhpnyet.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3epdvqabj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3hrwmljcq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3npcoymop.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3eumdhrie.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3auddrdyr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3glozxnjm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3eeuruuwq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vohrecji.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3dqcnjqbm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3idawpiiu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ljnfgorv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vditjkwy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ssvlenys.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tkjtispf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bzuywgvh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3dxvrioba.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3idzhfbks.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3nthpmomr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qlqtsxhz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3mnvivwbl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3svnockxs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3fhjxsxcw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jorerlsl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fnleauhb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qhsymkya.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ugtueoiq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bgkaaxnl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3sqgvacng.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3kvimsmbx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3eekoqwnj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3htfdbtkl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gvzlbvcz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3pncdycsf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3itfeszwk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vhjcfatr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3thumheup.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3oywfhnlg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3qtsszphy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ozljelwx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3krvioxma.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fkpdxgdw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3aiflllhe.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3adootcsk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gqurbhqx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xaejybqx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cvfmphcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exyjhwns.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3isjacapo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hhxtnniw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ttgbifbf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3pzimouft.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3arzrkmby.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dbvsyqnz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3afzxavbx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3dlsbmftx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3enrgpnzi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3xxfsbkre.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wxdpbyqn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xihighby.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fanazmls.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3axfjbmmd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wlgcrnju.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bnrjuqxl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oftslvao.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vrfkqwsj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kiqjkime.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3mkwhmlix.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zqjihwxf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3dnsflukl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pjotouvr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rzdzqpmr.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3plgisgwt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sjfrsdqb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hrnurosi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3jhrquuze.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jaugqcgn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3bnsuhbjf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aidxspdn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3pbmyjpye.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3omsmeuwh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ollybnhe.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mdycfirc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3mpyajact.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xepqnzrd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fxsfmdtr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3jxftoczn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3kyyzioja.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3tagjuqmr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zzlhvvwp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vrpwfcxm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tnaxfbdt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3qxkowwjm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3hhqnygzm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3icrttlgh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3pnbqzwol.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3sexvurtu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pncrkygv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3npiogrfp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sfdxtyac.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pepxvczb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3abscwrqw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kojotigd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oinkercn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3qzomtuxe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jrcxnawr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gvbrmtea.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3cnzthxfq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3tauaqztg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3loijsfth.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3nzynzhnh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ejtzaplz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3sydlcezu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3crhhvags.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3scotnzym.html


<!-- 参考信息 -->