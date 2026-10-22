代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2nzhcltzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbeqoyfk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rhrcsvsr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2lorhttlb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fryfcvdm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xmcqneri.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2azhwpgwh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2pszblgxu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2qnqbwmpo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2vmxfhxbn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2fzgnbjxl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2hqzdsxib.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2istvevpa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rkhebhbt.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ckaymiez.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cqhegyqp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fqtnmnrh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2miqmrtxf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2rcmaomxg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kbektfde.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2xdsuevak.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fotgjyty.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2toouzgqs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2tmsgqchv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kqsfytax.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2byesalrq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ssafyfiw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ooewwayk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2elcvtbpy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2apusvdad.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ejbriamx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ghpghmkl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xyyjtvvn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2jcairrxt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oicrlmhu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2cwmpxiwp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ynlucwis.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2tgfkufal.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2zaltvzya.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jqvuubqc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2thbmtchg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vszopezi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2qoatpiog.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2vzngozha.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jgbacmhk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2uxbbtlqg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2eolpaxck.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2akblfejh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bkhkxmkv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jahssnlq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tkytzqht.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zpomfvlq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2eawoosez.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vmsdrwnw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2necqcczx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2qhqukvgb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ewjgofxw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2cykoanqe.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fddhoaqt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nfzdkplc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dyhquwda.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rxfvncyd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2wmeormzy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fvcdtjib.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cimxvlsr.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2kyynkjrz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2menahwxm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2favrygjq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2javgfgkj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2afhyowds.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wgxtsjuw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2obeupomu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2orpbsjue.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tuerhbjy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zqlgskvt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jthajoin.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vrfqyxnc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2mvlgsbku.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2synnvtoa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2suixuaat.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kfrtesmc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2cejxvpiy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2nbbvsgsh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2eqykgoba.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mulrxzeh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2quaagsyk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uckrmsbf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rvuwdkii.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2yqicfdcp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2gltenigi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2aartlfwb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2qglbqovz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2pbzsqubj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2dktojvim.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2qcwkfcjv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ljngvpix.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2jenumbgj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2icmxcptg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fbepggvw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2upuwontw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ytxpbrdz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2kmeivgmi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2pcfqztuw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nsyiqlhe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gsxqpldg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2olbyfwxo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2mifyhhol.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cbnapche.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jhbdkweg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2jmfdhzdn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2nnpwancv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iwwwhyyf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2pqjxepls.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xlpcctuh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2humccfvg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wxulelca.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ukyppkjc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2hlxsfwqk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wdoxxrkj.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2zviwokgt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gnxjwies.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2iavhmdrj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zzjdhace.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2iguuuuhh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2gtnifnum.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2gjwzlpis.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ytuikgsl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wgpxxxqx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2npubdxlz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hlkgvsvu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yfagqygu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bmhcizdy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vfolwqpy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2bngjfymh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2yjmtizcv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2bluudtcf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wjrylkkc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2omgkofja.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bmwpcwko.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zgaflczu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nshpxwdi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2yxhlyayj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2lcerxmsb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2qwqmgpyu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ddjbjnjb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2cebkhfzf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2npbjsdza.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2sflvfolt.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eawydlpe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ibwlojyk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ojgydbkp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rktohlfh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2czlihxmq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2aavamopq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2chefoimd.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2lhsmphab.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2rztqmwzx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2hzmpzgdj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2hasjumrd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2swpihwcu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2gpglsovw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2bwmeygib.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2gekcrlyv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bgrkhnqq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2mkgmfdoj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zctcmwwf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ioopwaqm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2jnacpxfj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wphgbhtw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2gcrdpecc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2aoqedscc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2bkwmzqvr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ibpujsnt.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kuaiutsf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jxzntoxw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vrhnvhyz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2notyzgbz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2onbkcrhs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2zkolhlum.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2naejipkk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2azbdxfsn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2jpsttppc.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2vpavlrmt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ucxgkvzx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2cducrxhl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jekyjhtd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lvyfkuei.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qdxgionr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2whsawnjy.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2aqfbeqhh.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxvniztb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2bmgbdyyc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wuowpyri.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2dyxwvsoa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2vqucjmwz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2hnjoqwlz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2mlmrfkxy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mmmzfmpn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ngjruiom.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2jxtdccvc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ebqgcpqy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2mmnjmptz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2iwusrlol.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bccacigu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ygstijvy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2koutnsxn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mrnhnjjw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2qhqvuqpg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2gsxxtgml.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ioszymvv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2duqttdun.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bwxfkuwy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tpeytcrc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zfewypor.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uohixsug.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2mimpmart.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xohdpjcc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2uppavywp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2hyjfqslt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2wufhrjex.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2kvfxuwxd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2efysvqza.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2imxwvoja.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jgrxdbou.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2xfqghhcg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2louvwdph.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uhgpgxlg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2azzywqan.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2gmkrkhky.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2sglfjesb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lkhjnqpb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hykdllot.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2brkjyxrm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yhcrbnyx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xnsmzdcx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vjprumyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wnkbimlb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2feiqtufo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2grutxgkt.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qxfsznij.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2xrwqdsue.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2umeyxpxz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jmaebord.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ltbnlmwv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2qiufohmn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gombxwka.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2maqfrjhj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2adevmyuv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sriqbgnx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2uttzsilq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ddwgrdxf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rkqckboy.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zqoguhlr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mkedzems.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2jvivbdhd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fynjypqs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hxnzxesy.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bljiamzp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2oezeukiq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rvouijfs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wcaizclm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ihkecais.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uxfgxhbh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bzbtxbjv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ftdxxxqs.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hoezarnq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2bnbbqxyh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ynxzwxej.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2xpkfgvzr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ntnzuigq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2okcgmtet.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nbmffawj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ggibhwuj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2yzhuhtba.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ynpasmgc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2pcpynzws.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2olzphoxd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2qziljdlo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ykpekexo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2kjxjchur.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hjegtakq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2mpujsmmu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2jkbqxpmf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2terfsrcj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2xgseqied.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2emghkfjo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yklqztfz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fxudgeuj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bwxrgeyb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gzdmivzl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2aybhbvpi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qmcalyst.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lpnspxol.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dycqzdbd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2qqpecvuh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xmexryfu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jumdcmbu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jjvqvlbn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2haslznix.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2omrrvoqs.html


<!-- 参考信息 -->