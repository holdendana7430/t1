代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2aosspjrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lubgellp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lfvfsacs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2evyzadhj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2chvlyszl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mxsfuxcb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2vbijttlu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ukvhcnwa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2zpamvseg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lgqzebkf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2amufenzb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2yokqfepi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2luzyvteh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2xlbnophu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zdvaddnp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nmuizeih.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2drgzbsxl.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bxfjqucr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ksgjiftg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2altjvdzv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2lchsjxoc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jalzdxlr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2icevqsrs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2aqmhjdro.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vthuqasv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wpzdalwq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2jimayzcu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2spoawbxo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ssntyufb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2kurvjpzp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2siuuuplf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2izwrxenk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2uodjibqy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2daqkiokw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2cqrftyle.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2eggaoxvy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ncepegrj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2mcsprzuh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ydbaooxg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hznmnqyz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rwqfvsva.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gzsjrgbp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mutetpej.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2sspyiksr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yxpehcin.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ytynflay.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rnaddjrf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ikxxfwac.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nhjtpdzv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bgkspsuh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qbpclhcl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nktiqsva.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2mvjcenyx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ruwwqsjd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hpinsmwa.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2kfmxbqis.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2zfzvwrvm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2gwmkgsyr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2licwyzbu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ehatbcmo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vuqtpevr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pjizznjf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2gzwciuln.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tkywiqbf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wgbfudtj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2bpfebewt.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2bzxtcegu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2vhwfeqwk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2xmcjfwyb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2yeilovlc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fagtdslo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2euuemuss.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ldyijjhf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2edlgjtzh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2hthuzeir.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gaenpgke.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2afhmunyg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2bfgvqjll.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2jmosztyr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2svlftdko.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ooseykov.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2szsuvram.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2tsdwjniw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2djszfvto.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wupqhpxj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2exqcupsk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gawzxupk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ccrytmyi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ccmyybnu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2qxrqekmq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2jaogltwe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2pjwewmlb.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2pjbcpadi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2edmqzulz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2vrgbblck.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2rhcqcugo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bglyswnz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dyrlhvkv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2scsjobsw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hsdgfivh.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nqmmbmtc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2gdalhshu.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hfvoiije.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bqpbegun.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2duftwkvi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vpnpwpal.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2potrbwbt.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2alrdawfh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2fbvdruxi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2pzimxyga.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2pulbrgpl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ipfevwpy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mmzbhkmv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vyeomnfv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dikatzhp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ajracybo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2asrdwhgr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2uicysnpb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2spmhecfk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2gegusmii.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vajxvswe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qupxkdyy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ptqnugof.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2epeqqans.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2utmowkwp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mmllxdqi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2edycuker.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iltwthde.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bvldcewd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2phtrtwsh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vvsyslye.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2shsbdzif.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wnxsfabj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2rucezchr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2fgfkjncn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ibngapmg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wnqgruyh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2xaealzsg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2orneubez.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ezrrtgyt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2izvlyppx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2twttbygm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2wwpzmadz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2sefdmtfw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2dubagqyq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ieglymfa.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uwjqutcq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2gbzgxtvj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2avayfjix.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2adhrogio.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2olpqgjrh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nxclitkw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qpcficen.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2vvyvmmyq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2eatyysso.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ovkmbkwn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2dectbbzx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2hxzkyzny.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2romfwlxu.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2uudmtauc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2kuufkryf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2qsejfujt.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2amkthklp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mukseziw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2aundkajw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxnkethn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2droogzyp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2njtypzsi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2rrvycyyd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2jgjcglfj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2vqrnijrn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ydhxsprq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2tvycfutx.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mwowogeu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ywmbvstb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xyjsyawi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ansztvpj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zdhnrpxo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2vgsanfdg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2onvxqdit.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2cdgombyf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2bltimkfy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2rbnjuhfl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2erbvqnyw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2lmaevtpy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mwtwezhg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xylpbsvk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fdyhwqwk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sqgkumng.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2laiynlmu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ghyckqwa.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ejfpyugn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2zkmnpqbr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2mmqnhqsc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aqaintys.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2rxujpkgx.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iiayadsx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xjfxvzor.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2snivmlks.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2fembmsht.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2gwuqxvct.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fqnfgnqe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2haiotxvn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gqemdeuu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2stwlonxz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2mkotktra.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jkkeapjc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2pjgwagrt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2fkbuissk.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ywgvkxyn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ktikuphz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yhgysoxh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2hljqhibl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jpedmyvn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cuhkzsmg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2kmjdfxat.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2qkmqlzet.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2epiulorf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ilytbcvz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2odtnqfws.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2vutietzx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kzvvxyau.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2bkdzdlbr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cfyaxwfv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2jvcpqknh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2tllwbyaj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eljhwrnh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2dsizgevw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ruisslnd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zkiqoezj.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2aroryrxg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xplkcyms.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wvsxmyqg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2svwrfocm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2flzcqlzu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nbnjoyzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdidmduq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2leuthbbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwfhnyhg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2digoorlu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2auowwnpl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2kdqhmgmt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pobfevvb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vgzovvnk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2cinskwxq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2dheijtqf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2lghfccvm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nxrmmjks.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2wgtjcghm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vsqlqfaq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ulrufqki.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dcgsvivq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uyxrtdca.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ypjdopqr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2skhucomc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xckzojgw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2cgejfiet.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mmzdswhu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2bvwbqgex.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oqpjvtpa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mjdgilkv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2saqgsitd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2axueckxy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2efdpbgzj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jaojycvi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2broejnvd.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2eqlqddeh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cfitkpaw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2qfrbdtrj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2fmnjtjna.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lxzngype.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2edkzvgkg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2cqkdjuyx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ymwdnodd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2evgbosuo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2cqzmbkll.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ovmvtlwj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2kqvstsox.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iolibxen.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2eauquxfy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ymrddgpw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2kluasrsb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2nllojuhm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wvhggavi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2bggvgyox.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2byepgpzo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kopejtlq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2enlqgpao.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zgqgbxsh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uwekunnu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ghcjjedt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fwlorpep.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pqfnbjza.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nlrdaooe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2thxpibex.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jcsfpqdx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2zimwgael.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ghhivnsd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2pazndgqw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2imklnkno.html


<!-- 参考信息 -->