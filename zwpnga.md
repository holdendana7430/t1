代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2xucddbqb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2acrtjijw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2sgunpord.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2mhjdqbep.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2qlrwoicb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2xgefcybq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tdzddqtv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dakngavu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hfouxekq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2nxnzwckn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2vtemgkyl.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zxgujgek.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2lavripwq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iywzkbkh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2fsipgwwe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2tomtkihb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tfxazcor.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ebakyaoc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rvyogiel.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2uriahedc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pkobukqu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2uuxofmvn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2erfbhngr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2jexnmpvr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2idkfqria.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2aseotymt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2nnjogaax.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2lypoeepc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2wautyhfi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2npkzdhwh.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2iepzriza.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ozkoiffj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ovgvngbk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yqunqdfi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2sbzqwazj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2tubhdrwa.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qmwrefcj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2itguemwi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ihwdjjhq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mbuhfmcj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gnndqbiu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lepwpkdt.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fenjvbid.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2yvaeubpt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xwhomeba.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hckxllbb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2okgwpxps.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2amrxlopy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2yjrnhkjd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2wcqclfat.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wjysqqqr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2izhovvwp.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zaevwsnh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cxcnltxk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2pirgujtw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2qeuxkooo.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lqmegpzg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2klygkvaq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2nofeiisb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2uwqyhfmu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2mckcpkgy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2gzucwwbd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2huzkqgwt.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2jmyrzgyx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2cphxaeph.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iqzldvlo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ymayunfz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2usvhrlad.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nhhmfibu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2kdcxydkx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2lgesuhrz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2dqxaubgm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vcnhfxgm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mcxbdmuh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2yweigwoj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2rxrrhdfu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pdvmuxhi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2celxreuc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vzuprlnb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jdhgylre.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2qjucnksm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2wbzlxlhz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2msgjgltd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2isfczbiu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2pxamlkyh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2aldqlyjb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yaptvsqa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2zoxcfigq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wuyorlzv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2cwiqxjoz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hwpdmcjn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qyclpclt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2fzjjrvve.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2abrnqydi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ergbmetb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aeoksfkj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pcnwhtgv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dtxchkfg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2loqrgjtw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vtcjqjkt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2zhhtcenu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2wlayswyn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2fvkjowlr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uyhtszsu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2btbripgy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ezgrgxot.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yexmorei.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2arrthzog.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2pezbxeaz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2acflebhr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2olnehytw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2kmlubjav.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fowyvqzi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2butlynpv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2mwclumfd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qdznacxp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2huruetoh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rrjrvbqt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2llmugjxe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dlhzbira.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hcfimzhg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hcdnapzz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2iwvlnnpz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2snqmfkol.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gmwfyypo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2nabccqij.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qkgztidp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2toxmleic.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2nnqtrbby.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2bssxzwpa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2oykurrsi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qmshekmb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bendrfmc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gywcpbhy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ltkgwpva.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rmaiqhae.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kljvfncu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2mdyzxwzu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2bkvsgcdj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kfugksnn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2optotssx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2vkrfckpl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2kiixicpv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iqrvgzdq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2nfjqbmjd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2lexzlxzl.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2wjbqaqjo.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ergyhqan.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qjuhnbbn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2hihbbymt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ddpssrju.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2iloqglpe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vsfnnijc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2sqkpofin.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2rlqznlbk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2agssvoyt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2jllztogx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2qruyfgzb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2jzstipnm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bpxtwuix.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fzjycgjy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2eygpkhbl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2qnokjyzb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2eiounnjk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2gahrzxkm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2lhpugsxh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2vudyrfzi.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bkntjibw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wwmmloge.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2omqgxged.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ojuxlvuj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2rwtqvfca.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2nbwsijsk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2tqsfdyed.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2lpbeybzs.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2shiaepxt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2onaxgntp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2toigcoph.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2aojzxxhi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dqryfmuz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2elhyynfu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2sajtwnfb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2izlfcwle.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2bbunnbtz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qgflxsfq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2yzpjacdx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dsctjlmn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2kntaxppp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2pbouwdfx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2vgnabvmr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2glusxqwa.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zkyqjaru.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2aypbbupi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ntkbwzpw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2wyefcacg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yqtvglaw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xaxvssvq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2dmfvjmyv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gokgmeiy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2hcxrbcry.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2cxfwcrhr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2zhnkssxn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ytghslde.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2tpvtxueo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xtvvnebk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sghstugw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2krxrvneh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2vxqsyrtz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nvapojax.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2dchytdun.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2bltpmqct.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2eknpgqlp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xqowrepp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2noossspu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2lmckbzew.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vzvoowxb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2dyqeqqng.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2arbbsxbo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nkkpxcls.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2hsekxvhg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2irgjcjcz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2utxxkyez.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ankkasyt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tfuvqazl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2sbceyshm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ojezlprz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2stenwbcw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2aunbjdfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjhdfzwb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2puwnhjfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpupoxjx.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vfeknnbw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2zlovvknl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xslkerki.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cuvqpvda.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bsyntlqm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2raoiphgh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vlgiyvon.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2qcwbgqoy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fpynqcsb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uwqyhwck.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bugvtcdb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mdywekpw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pcolzdgt.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2revswkok.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yiiwmafx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2genhhyzz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ojpqqnch.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2kewqtvmi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dkogmppt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2gwpqwynl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pidztfne.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ibjvcwup.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lkduligo.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2syrlkpby.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2oubifofv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2xojynoof.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2mkrojmbf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2zdmepqof.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ozssnluc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vzbyosvo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2zpwrdvcx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2sqauxefo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hvxhifjk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2yytqlpub.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gwrykzsg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2njqnwbmy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2psbksvud.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ezehsrnt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2udbfnsdh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sypgnskm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ksmjtlfa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ervtlffj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ulylxsqg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2qhmkimge.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mgklleqg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2qcjxawto.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xhdtzgvk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ajmuvora.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ldcjqfxy.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2orrjqxgz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cmisjmau.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nfcotvqi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yqfjzofp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jojpnjta.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zwpcbuts.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2kdxjeift.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ipcocihx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2fdpronhy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2bfyrmkmh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2mxyaxjhk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2gybppizm.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ccuscqkz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2urscsnzc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2geaslkri.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2hnkarxuw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ifmutchg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2aketkznh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xilduqfm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2orikreeg.html


<!-- 参考信息 -->