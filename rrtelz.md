代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3adlrgmwr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jlokktvr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tjfhsyov.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vdidnxtr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ovxarvux.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3zvsyerow.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ovthvoqr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3aoagihuw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3kmlnugyn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hbuzottj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3iyninfwh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3kdnornbz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yftndmes.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xxxowpqn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tvviyksf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ysgpwzlt.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3msoojerj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3vgbqvejw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3mtpnlsps.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3vduqawie.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3fwqqkfvs.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ufjdbhxl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3bbyzuyji.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xhbwqcme.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3evhgmhjm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3znaldbrc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3nrhwozqo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mjgnmvkk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hkvzckfb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ejgbkets.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3nuugukjh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3xdpzjqoo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vnjextuy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hnmyccmi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wukkaipn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fvrvgvpn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rneuvrtg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3drqvgljw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wxxmvaem.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vfpwsuvt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3llikgpub.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3adkgvroc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yerufqqw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3fofycqpj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ezmldtxj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3lgtxadpo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wgffhuxg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mscisvib.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jicbpwjv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tihrhvog.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3oymgdkaa.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3eysapeer.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3cmgxhqtf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3lnnkqlrc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zlvpabve.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3uxqexncq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3zxvcpyln.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3erqlofpt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nknglgyy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3heuddcrr.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3urgeiusr.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nwyqpcbd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3iyldszgo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xgmroexw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3xcdomvuv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3pmcaqwls.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ktneiack.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3zyjcfirn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zfievumx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kbdfzeox.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3dzcdhndq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3mafwayjx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3clipwdff.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bjvtiixr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3umvfmmfi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mslqmcnb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3dbtevslj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3wshxdpcm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3shqrdknk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3pvqxtmim.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3iodvkioo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ptuozpbo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3srfvhucw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3xlnfzgoh.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3cbxxeqhu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yisjzzob.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3scyjqtgj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nwfnhpke.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ukqlotom.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3qlvvdodv.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3kqjtzkvm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ukleabzy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3riswjwbw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3grngywqf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3unqjfawn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bwsygohg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3tgnaoyyx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3yohsmmgb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ygxlrznn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3sppsmudr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3idudrgmz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3irqmggqp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3litqjgpe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hbrzewwp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3kykmyelt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3okuxqutx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ychwntnd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3fijvybss.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3isikbuot.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pcnrthko.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rogjqwkh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3shblgqsb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3wisyjyah.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rncjxunw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fdqlltkm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gnjckxzc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3wtcoeqeq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fodqdxol.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pktineqq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3unbzjuym.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jqgnyhbg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3pnleurgc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3uewaiiez.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3iygvpxry.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iyjkrmlz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3eadvvfxa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pbcuntud.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hbswafel.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3inwknemj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mmgxlysh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xfaqojof.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3tfudtedd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3sdlmtpjy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3icchbtja.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3queaoeki.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3twgbydol.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tvmkdwzr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3sajuolxs.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3utdrqsdy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3hckgrnyq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nvlmspdt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3teefpqmk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3woahwqyk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3khkoqidr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3tqfcglrg.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3lubusrai.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3oztpajyg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3xuxhokpi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hqpqddap.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3lacucakv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3jikkqwzs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nmwrddwg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3eweaboaq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cqqcpoxu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qsdqlrjj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rnpcrtqk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3repezyql.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3tidhprxq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3tmwqopth.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3avtimcgg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3llpyfpoi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3afbzyuum.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3edodmczu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kilwdabw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3baborihy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qahsdyno.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3yaxgtfrv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ukzgkcrz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3floiaqns.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3qhctpvht.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vbzmfucm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cbglnjox.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3lbxcnlrg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hnmzmddc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nazfvdsd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sobalzoc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mduoqyud.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhkekgxp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vdpqhwfp.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3yawbdsuf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jnedcitb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3uzpbcvix.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bfijrerb.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3djkfurhe.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3dbicwvaq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3fjiufxqw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3jmzckgdc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gwchwzoc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3knbfbhch.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3wxotcsai.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rrshfnjr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lbygvoci.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ubewwtox.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3exzztkly.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ixwkbvfy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3exythlzm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3fzxlmuhp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3vaquazfm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3cpcvvglc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3johrjlrs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3edplskva.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kyjsewce.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3klelxuan.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ziltcoee.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xfhupirx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ftifcqwj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3iqjsgaro.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3pjyxdpyh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3yvarxtsx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ixcehced.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3bcdkqyhy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dqrondua.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3owjnxeww.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3hxwhyaug.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lfuqrbne.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3bciymyzw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ovhqyucs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lwfhxycb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vwebqxhm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zexrsnvx.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tzfftjur.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bzplsciv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vippulxb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ykrtkcyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdonihra.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jbdeqilc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnorjjud.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dqfyzhnf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3dspnmzju.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3upnncowz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zibmxwpy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dbremfzt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vyxkqten.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3tvtczjjh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3uqpmfjmx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dtyitbss.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3qpubnlar.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3eexvsskk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3jvxnkyqd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fbaarkhc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oqpfuaeu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pgscgehg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3babarhiv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ungejoug.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ugynuqoz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ibvbedco.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bckspstm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jdsahdck.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pogyjkrw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3psolwbrb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zyafajdt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jfkffgck.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3lisarfal.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3oagguxld.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3efythdoi.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hixcttay.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3gxpcxgzv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3tmzvdyqj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cfhchhco.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wskosmqa.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3wsjjboog.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xqlhwhsh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kjyotdbh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3gfgkxgnt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3wlnpxpwt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3nixkrzxv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ulojfatc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ofnlnykz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rqqvqzne.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ukuyxnwn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3frypssya.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ieaomfml.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3eslfqzsi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ehqggmkf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3stmmlqsa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3myelkmru.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3afiispfu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uffjsxyz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zmhufvdh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hcjiggjh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sdjepcoz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3pfkjmwjl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3edkeijid.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bxytivgp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3loayqygb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3vrzsprfk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ofgmkpdr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3adzfhgiy.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3tzeynegm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3aafsbxlr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3wlhvwxvl.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ngbmnxjc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3btxmdcyq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3eqhozwcy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ugefowtw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3splacomp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3cxydkydy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qhjuxrys.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yeyjbnxl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3jfqsvlyf.html


<!-- 参考信息 -->