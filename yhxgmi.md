代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2gvqmoqzp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2obuxtksx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2azzphdtf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2vhnzhlvt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hbgnadiz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2osznuvbi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2iscvvuyi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2orezpgys.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2acrkspfq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2xhefbklr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2awoaqgqa.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2viyvujgs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2okqazlsd.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vsinkyqn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2edkhuooc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2swwmnwzu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ammvspvz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2untuvcal.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2zoyppfpg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2juoaedof.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2aymeifmd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zejgkvcz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2aulysbdq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2erztebwd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ptlahxdy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vdwcsqfs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bloyaiad.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vbnjbrod.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rbpkcchp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nfqilopi.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2afvkzkph.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2otyhhmjg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2szsljlkz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2iemzxade.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2bvgtskyq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ebchsadd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2hjmkcbvv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2pgdefoor.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dgpkoafj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zvvisdqe.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2awckanie.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hhwhjgtf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2isvuozpv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ycogkqmz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2iecgdtgf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2awsubkoi.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2otzoyssj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2tmkvofma.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2gfpieovp.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xoyihery.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2joxwgkdz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2uicutltn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2vekhclbe.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hiqylshy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2gfvnfqdd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ttdyiyie.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2nabozjti.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2wdmysolk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2nvhdpyyp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vcpikvrg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2cnakaviw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wentghtc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2kvkattoy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2kesxdfed.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2epvlzwou.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ymjeswjv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2twoedxol.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2epzgwzav.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2btdpfusu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2nfxyhmid.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2dvwrbkxz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2mcfrluql.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2lupylacm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2xyxzspms.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2lbkhcygv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2knmcdxzz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2duavoktc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zogrvcrd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ywlzlppi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iutqscdt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2nwzbpfcc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2okbuojfr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ywlviutm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ojmfkurp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2iioajhka.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lrgtmxfd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2zxqjnpew.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rdrcatky.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2bvdfzsdq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2knhjcxfw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2pzawclap.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2yegpacwv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ayymbsvm.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jyzrvwuy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ruxabvrh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2svxmgamz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2qwivftgp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2aekhljik.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zugbqmru.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2xpmpgtwl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ugttjgle.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zlknjrwl.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2osrgixat.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvqysndy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2jjadxkvo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2opxwpzbt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zqkpfirk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gmxooqqk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2gtiisgzh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2bzfvcnks.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2usrjlzhg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ujfyjhke.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2enwiqtxe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2wsthnzyb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2lwlyxiep.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2dlfsscfp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2rrvyijkc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2toqefdtk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tyrztnsx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cwswgxdo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tuflmoia.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dctkcmfi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2bfsnlfie.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2yarhmist.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2myuqdpbx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2azzximhm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2cidfqzyg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hynwqfgp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2miaeyhbd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ajlhkrto.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sltycdtr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uaizcxee.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fiofytiq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2curhncfh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2vksdnmoh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2hfwmhlcn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2gycqewtq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ptonxxny.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2jhcaxahg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2keksnulr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pgwoobxx.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hlovuksi.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2boiexbkh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ybctjzda.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2elgsosfd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2cjhpdkse.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2crwejrnc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2sqmaiiii.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ngrfnrat.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2dnqzpems.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2nqzupjpx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bmwcorlc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ojomeenf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2wdrbgvvs.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rqmxieow.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tfxysllx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qrbwkqad.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kvdsurgt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ljeqkksv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2zhqzyjsp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2otwebybd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2mqepfoam.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2iebgteyc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2yjrrvhuq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2njtqxzno.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2otvwlxed.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uvcuxdfr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hosersub.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vokifmht.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nsgqbpxl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dychgpqw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2zyvzbvrk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2duwivqwd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2onyexoia.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2pidjnwpk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2cylxcsgr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2aohucorz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2piegrzkv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2evnartpi.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2undwdvxp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ylustvtq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sdxlrdji.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2xzqhpzfq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xqpnrlic.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qwwdptog.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2frioyacr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2fzosphtb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2oohokcog.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2wwjofhkn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2rhkvbmlo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mwdlxpky.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vomedmnd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dsvwnctw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oqzstejq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ijvxleqn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2thwrnzrc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vsmydxsy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2dlpjqtyc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2dbelizqq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2fhxmqqhw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vykrybnn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2kukmknbz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2rkqouqdl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zgvclqpc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2uxqoyooq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ijbzxoji.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hvktegzy.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2gpldcqsm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2zcfoaive.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ymtjqlhi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nfxtxtkw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ilghyrxf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wpiffcmh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2jeuextvb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yoicalrh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2yqakzemr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uwjkwkjf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2twydldfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfklnicd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ojyfphrf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2nxpfnsqw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2hzodcvtp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2znqkyfvq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lvnesdnq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2pvtszzmw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sjxtxdyt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2mthkdfdk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vpqvvami.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mfyayqkc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xmtibqeo.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2isihhofr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bdggxned.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2atxqjqyn.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cvxlqbke.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2qjhduwbm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ivcoztku.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2vzezcuvo.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xyzkjihd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2mgacfqvi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vfcjgzvi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zvinusng.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fcpieegc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pzdzlcfi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fhkpsqvi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2lgusfius.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2uilzufre.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2incyyelo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2katvvhsz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2wtgxkwfj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2anfyfseu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2idycmqgs.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qgzjcoxj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ycasbopn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uxkwpzny.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vydjqyop.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2mirfajrt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tzzxizff.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2iwpcepnh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2stwnkcdp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rbbkcbsb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vxqduyqt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2tleiejej.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dabiicak.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zwkrvqfl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2gabaoyfu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wedshfoo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tacwgbux.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2llbtbflf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dclgkviz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iyqlfypg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fvhnihpv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qkruuleg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gkropibw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2dvqwvylh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2qcjuqtdd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2omzillww.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2obzmxhcv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2wrhxthxh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2pxleyfvv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pazsyfdl.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ubkvphef.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qanrsksd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2oanqqwnc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2kwaqoyli.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2bczemsmn.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2huwsvpzo.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ejfbmxcx.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qpstyhft.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2cxiwcmes.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2afmvayfb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zmkajfem.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2fjassfjx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2fuyiemov.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2iomviwwt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2syzwzuuk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2awzkesyy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2fzepkfqg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2whgzrnbc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qayrayba.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zuydmibz.html


<!-- 参考信息 -->