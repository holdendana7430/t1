代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fyougvlc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lrdmhhcw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2fdialybi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2jihwfqbt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2kivwsrbg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ffvvufvi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2gdhwxpkk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2vodglxve.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2tnroalhl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2buuoxgpb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cmlvfzqc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nzajduoy.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fcprbcrf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2tsdqqnqi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2frbyrkze.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ftrtvead.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2zqbqcdwp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2xgvpyqqo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2hrmbjvgi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vznwxplh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ibcevptn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nflhdwzb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2mlujvhgp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ywlutubm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lxyvugsj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jhrcrvjd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hpplvqgc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2irpuxzxh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2gborhzbh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dogxjanp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2enkendbm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2dkakzkyt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2devlcqpp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2hsbwfrkv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2sakzzsmi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2aielekan.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bqfgcqnp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2sqiiyciq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2mhkoqpkf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2zjgyjzwv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uwusrlpf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rsmtwqir.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rgixxmdd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iiculjjl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xorjtqim.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ytazfcwj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2untfrwbx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2plhyjcgs.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2cwxfkrmd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xnieiukl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ubekqbsa.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2sukzvxop.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2bzhjvyoo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rdyixazr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kbpjcmqu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ypwwqzms.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ztfameto.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tedqvnxp.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2sumijgeh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2xinhnkhn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aiimckqk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ajnzxkzp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uxdykvhp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2hyuhxgng.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2xhxqibie.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2dheblhrt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2lliolhyq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2orcvbiua.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xnafkhqv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nvhtlrfj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ruyakepf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hyheascs.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kfjbolby.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2gtrtiswn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2hulcidct.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2rzduyzab.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2iljkflgm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2aizdwaet.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2oanfnnxz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rtnhkpur.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pylebhcn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hjeepbxi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lmbpuaqv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ntzdasnj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2celxyorm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2snypxipt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2dleeerqz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2djltgkat.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2osnbrnym.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2jdesosnk.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bpsyruee.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2nfjmjvoc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2stnanula.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tptkmrri.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2tisgrrki.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rqlpbnqn.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2npxxegmc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2jpotinco.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2sonpkutx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xgsqcjwk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zxwhjhuk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rvesrlcn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2hydqyoes.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bsoxjcif.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2mkunllvt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ersthuyr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2vcxnhrcg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2jiigbwfb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ellljhcz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wpgulunr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2odopsufh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2yzpcblts.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2kvufoufr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2rxrnzppd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iqefdwob.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ujudpvpx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nquqhalw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yuulfzmx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ulhzdyrh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvmjuheb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2zkkrqelc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cexugwyq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zgvnfppg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hncjawbg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ycidflgy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hdknldse.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2svphpjgx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2uxveicym.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cmrhnfyp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2szgrgxbv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2wwozcvxj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2aefqhzwc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hwcxrsnc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ervonvlj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vxzuxaaw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jxbjzkvm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ichslrat.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2gevuqmlb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2pzrqdnzk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2lcuizfzq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2fzupcdww.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2rehkkqug.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2yottmvzb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dsoepwpu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2qsboolef.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2uutjdykw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2oqrwducv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ryxnwrov.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ggvtdyen.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2dxuxznhp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2pglieucp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2dugjabkt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2loygyrwe.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2deoqyzbq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2hbtqubca.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2mrdgxxtw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oyxaaaav.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rhejpnxo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2vbclvtun.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sjnwozge.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2bkksqzfl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2owqelimg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2wliaghyr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2oenkrskq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jxbrxrph.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2snojuvma.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2codqpyek.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2lwxcakif.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2mwfwkkpz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2lvpdvhrg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ijtcxwok.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wanhcjws.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wmgzzlyu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kamtixxu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2yrdozfcz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2yffursre.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2filftlee.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2abesloqs.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ugjizfpe.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2xupneiyr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gvrqgsbc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wogwjdex.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ptvphpch.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nxogzfqu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hsovahri.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lpgknlps.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vmudpjmv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2iopmbawc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ueuhhkqj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2fvfkerkh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2kvzjirrq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2vsjkupbe.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2lzydndmk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2uggopciy.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ocsuuxrb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2chadolli.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2lrvjvoza.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2kpigwqae.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xbfhoqau.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2valshpaj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ecykgxfw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2durtkity.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kluockyg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2nbbdqckt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2sphzegde.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ivymsvyv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vrofdrds.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rogkxfzg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2lqjdulco.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lcytzhds.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2higoosyy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2bpdcwpff.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wfwpkhow.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ausswcsd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2koaxecom.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2omghsbng.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xzcutvpk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jimqaosy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2njaxbndy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jucmfsqh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2sztytzia.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zxslqjrv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2itqhqdaz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ytgduakw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qitnbnsi.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2eirmjljm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kgqxduai.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gczslsvm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2desukffu.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2idwepohf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2iunwizln.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qyfcknqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ouraxsoq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2bbjsulgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epusjesf.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yajafeju.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2xwdeewef.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2azrjvwky.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2skslmdpd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kfowherc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ogozxpzd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2snshpgbz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2fpztffje.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hkubkzzc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2rtodkzox.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gfzhuqyq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vgldsqbp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fjgrmxqo.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nzkekcwv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gxtxpeki.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2tspwsptg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2dcggtngn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2puirgdtr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gcphjwge.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2gbfwziqv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eadcarjf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cduipvbk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2epgcaxkt.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2chcqqygt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qoyjqfkt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2emsyofps.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2uohcarcc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2hxzveelb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vckfpegf.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2jeedkrle.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2dfkcxinj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ejrkfrui.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rrdyddsd.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2cwlwrhmf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2loiowrki.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qtgsklui.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2mwlakdrr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2gzmsrels.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2twxeeayz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mefttdny.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tpowphym.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dbeurfew.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2xhgsomvx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fndlzirk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bankylzq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2lqbryjku.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2piwsokkf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hpfwyrrn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kqriimaa.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2efbnamdg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hqwnrduh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dhxltnaz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yaqicnse.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2djchcnns.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2bqolonwh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2dfqfaquf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zkveqjyw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mlgwoxmu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2yfkgeqal.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2xkrcjklf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2dhpgekuq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2nosdejwl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2vqthutdu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2dmllrhhx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2iaeeuapn.html


<!-- 参考信息 -->