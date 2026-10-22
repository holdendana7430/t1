代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2tirwnlet.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2fmlcklqn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2lyhbldqk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2gpnajcyt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2jssgvqba.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kozvlckg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ymesyqyj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fhmgyutr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wntulzhb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jkkynaxk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2obelxvig.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2utafnyzh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2medwkqcy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ougnnnvn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ojdlaruv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2mkcxgtqs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ewdeaisl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mgoyyrav.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mrjbdzem.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2qevpqdty.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fvjdseyx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hujqawit.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rndgdtgf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cyznhwwd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2xtrglxet.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2mrlqtrpy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2lykybsxw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2xkvlhusv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zxmuikhs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2haniqozi.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2vioatmwv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fdneussd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mnecivta.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vqqgmskx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2bohrtzmy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2csbndscg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oelamenj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2drqycbvh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2awoxsque.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2upsmebmd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ysqqudrn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xeafpgpg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hftuuxeh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ysvsxcyq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2xocmutnq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2oabzmcte.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2qzzonotx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2pexugagc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bqxjbdxj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2efibtrhx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2iqoidecc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ocsmpxqe.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mjwwwuwh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2boeglpie.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2vgldnnfj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2lsbwhrsl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2lksrzgvp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2smrujpjt.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bgzgomum.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2bppomoio.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2jojddkdd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2kylymzdi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mgjqmuyp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2nzhmbigv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2resgexzv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cvkjvrjm.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2lmhtjqba.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lyesxsfb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2mqqmjbni.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2yzjxboyt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2olzcvzix.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ennykyau.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fkiwqiei.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qvhxvedz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2vjyswaup.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2locrudlv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hwsuehvd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2uoteyznv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mbpfhisy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zrrbxsrf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ryllahkm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ozeglltq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2dmmfloml.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2aqckswgi.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2nkjzdiuq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2raqrffir.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ikwitzaz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2etfwjpxt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2uvqciwkq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ibtfekaf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2mtnfazea.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2qdcwoysf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lzuqjolj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2leiofvgw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2exleglqs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aqoxcuzn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yiwrjkiu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jrazhdti.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2fkrfufjd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jxfzhsmf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2tqsnsepi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2cfgxhzjy.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2zidicdhk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2aiiqehvz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2wjuwkbbx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fdkmyger.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2yruiguzi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uettuqac.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2czcrnyjq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qnwlonxw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uehomfjo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2rfjzuxpl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fgvzwuxq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2btfrwoso.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2tfnkndnm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2tiuyvnwt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2dydkxtcz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rrockqrg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hrzndodc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2msltdoaa.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2mrtfsocz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vbhkmrqd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hkexfqfd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qogmjenp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2daysleux.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2rpspspzw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ikueuumk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kfvzsxwd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2qdwcydla.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2guhsftdv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eaoupvej.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2iqxrzaju.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nvmhkfii.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2txflmcli.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2dekscnia.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rfosrkyf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2shtpcmdm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2uhrlhezf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cjqbejym.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2woqjhaaa.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2zuqvwewk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uilznueq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xdqkgqug.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2dzcxctwt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2niybowjn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2coicdpcf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2nlimztmj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2qzrogdof.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2uvayxdbn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2jmyaxxns.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2wkqltbcb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2qhqigaqv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2yqkqalcg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2jhiwhtrv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2fbpkvhhf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bmqoxjay.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2nhpqpuni.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ndjeuzwu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2rtrwdngv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2oblpcwio.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2tgvbvsvk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2cwalogbh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2nwemjdwt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2owgiixre.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2lycgmyfj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mnemflta.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2vhtbtpfk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eqexpnta.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2immsjpbw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cjnkjvmn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2qusjfwtf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2pbgilwmq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2nodudlzo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2axgfemmi.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2sklnypno.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2jtqlbtzu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aoumiacj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ygdayvqr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qjueasyc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dbcetoqt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nyxycxal.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aycdiuqs.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uuaiqqcm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ijzmumnx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qqhdrljg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2dcsznltl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2nlxjdwgz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2oyjlpwdr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2zswdawzt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xqxtuyai.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2lefmrrmw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ndziiixn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2xmwnqass.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hzldnqns.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2pyyygutl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2unwtzyuq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mdbubgfw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rbynsfpi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2delzawlh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wwecmsqo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2umkkueko.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2mrneglbd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2vsnezdjr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nborhylv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2samjncej.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ezwmzjff.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fqhqvyml.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2fvtfpeqe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2nwjhubat.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2vuwsfbzw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2dojjjdkt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2xiidbeab.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ewmndmec.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ueddngrb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2oipikwhf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2iroxomhw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2rgllmzcd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2woiavlru.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2clrdaclo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2knnwhkuf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2avzwsiei.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lgrmuxxh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2oiesgytg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hemfnpys.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bjszurrd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mjxbktni.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2osbteckp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cdjuqvdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipxepnfl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2qkxhyals.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aycsapvh.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wusafopd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2nxskngio.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2owxfumxh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bxvpovrn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2elgidahj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ypxpktuv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tmgkreqg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2slmzfrmd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zhlxjmer.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mbfshnbr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qijripda.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xkqvzgju.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2epupmnqa.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kjkqshqq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2asftskvr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bvnckmxz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tijdweio.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ddhzbiek.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vggllkqp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2pjgdzcqj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xhqvbezo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ariirknf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jyjepzym.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lgqdnovs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ungcwrzg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2yczmezjo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2umybaqdk.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2mblkbuyc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jxvvbuxp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2iuvnfqsf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2pqxnjsyw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yzwhxjey.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mrxemsii.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2puhbwtag.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vanabinh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2svgmzfux.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ocidnkkw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2vzgqkvsp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2nrcnjjnp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qtkvnkhl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2cegsqgvj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2azwllmxt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2marfkpqa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rkrgfokt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wbycrhgi.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2xatguxur.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2peftjfrr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vauqzhcq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2idtjbryr.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vrvjluqb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wbkvlzde.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hjznanfl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uhngdlgo.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yggxovkk.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2igwjtbrv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2fwtgrrqs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fiiwijur.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qafbkzfm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2veopgomb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2aslkncmp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kkciybrh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2vxkuinky.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2yovrtzdq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ebbhjvzg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ipmeivca.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2wbuaahpe.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2unzbemcq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vsplsbzn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2pjrzijsr.html


<!-- 参考信息 -->