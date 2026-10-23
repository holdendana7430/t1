代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3pltrauvz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3uvmrnkmd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3lwivzkvf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3rmbiwztr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3numxbmfu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3yhduikra.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3wvzxdqgo.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3zgboxlhe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3hpyyudab.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3zdifsyuk.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fukonbyj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3etshpuor.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3icrimdno.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3hmucgsqp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3sdfkeyyu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3tdfmuekp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ujfhkoek.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xiatgrli.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3faegnpfb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3dskjfnoc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ekpxixff.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jgbcsbyl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ylvesfjn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3dzuiprhh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gfwluoew.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3msfwniql.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zzpnmrwm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3herwunnq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3kgldhqor.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3jczalmay.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3xptkvuoj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3qmelfmhi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3uuoxtsua.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3vpymqzge.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3bxfepjzq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hepubgzb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ekypnzvt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mlcdateb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3cwcpcgqi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3sicgomgx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3paycyvuc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wczylyct.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zosubuhm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3fuskmbqr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3krrzuytf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rcxvebme.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3orpeilrr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3npdmjooe.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3htmesrsl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dmokcoky.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3rpbswakc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3kdyekljf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3dmdduibr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3tgwnzmql.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qxvykhoa.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dmfbmtpm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ueejpfxp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3alaqrgcl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3rotxlmoo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3odtstrfy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dkrtlisr.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3mxmwloro.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3mpknodmp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3civlohar.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3lwvxiake.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3jyzowwxe.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ibgbdiyg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3pnquyqhb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cifsdwwn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uznpeaig.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3kwnekjop.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tvbopmls.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3epruhjuw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3rhcwdnph.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3prpicwmb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3amtdsesh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bexxdpfe.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3oanxkbke.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3cshegxwo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3fuxrejzq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ghmawkfs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pvrwwqdf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nbmbkjou.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3femlkwrj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3uyqgpquu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3cbydpgmy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3yyukugff.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wvejriov.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3guyzlygc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3qdujyhct.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3firhtkar.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3zykvslpk.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3zmlusfjp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3xqzucegf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3fuqrcneq.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xjdezmqd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kwsobuiz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3bdunrghr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3vxocbrqg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jnohvwbv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xprwpnku.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tykdkhts.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3cocvfrar.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rjiydwdn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3weoazkhs.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3igqzrviz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3snootyvx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3kkmuxmhw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3dxvcdsao.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3flhizdhl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ceccbbwt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gehtyuto.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3khgzezzq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3gnhpykyy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ylbotowy.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3adryolvu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3eydvdonq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3orweexix.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ihlxmcrl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lhvwixyy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rmvjloxx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3natxgrlk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3khrxoxoc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yxkguhce.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3nmfdiaqs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3efnvioed.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cgodhsrd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kpvxboxv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nlrhfrxi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3kaweeium.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ypetxsmq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3nhsbeanl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mnbvseaa.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3risemuez.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wbicgttr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wbkushsa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nwebjbjo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wujblucq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3txbhlrbc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3nqspbsco.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gyyfzhig.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3vgeqzfco.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3dosftvyq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kmikvwqm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3cuthehlo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3glrapphs.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3vksvaion.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3netkhcrk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tfnegent.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3vsugleaq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ntqpvcxj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3imwkftho.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3whzfgkyt.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3jbliyrxi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3osalwxpp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3epdywlda.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dbiuvenh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ghnhindk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3jczpnltr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wdyezevx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3quecogyf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ononnsdk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3lkrlcyqi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3hppqoaty.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3eggtrxfn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ihrrjrho.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ktxnhtsg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3qxdjvdys.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ygnjpsok.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tfflzzer.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nkbuqufz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hrxmetqc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3malyfjsc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3akvhevmw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3oyccwmqe.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3tavhjbwf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3yzkrywus.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3sluuhgrp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3waetffya.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tdycdfhw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jxcgketl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zsveluyz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tgpggeud.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vdplozkt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wxnwojws.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3occlfajp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wbtebzdl.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3hpaphmwv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ofistklm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3owcwwiob.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3jzaiscmw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ztoblkfj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tbufhmus.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3basywkfb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3vdbnafah.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3nfkkubjb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3yduqvxuv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zpvqitri.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tnakwfec.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ozthqene.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vfxjrabd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3lrgbkpcb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jfysudzs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3uqlihgqn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qxtibxgc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3jiqdgmmk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mxfhmunv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3iukoslbu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptphfqhl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pwnpiaej.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mytyuccw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3tibtdecy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mlspagyl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3pnzxyjhv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3rkghjbqa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wlhwdqek.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3guzsrpfc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qgxvvyao.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3xtspqrie.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ncncmevv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3powutrfn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ldssxdru.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ewpsmskv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mhfthwjl.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qdqixgbm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ytfvsnyf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3onwqwoib.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nfquczbz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cvqknyny.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rsryyfnp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hftdbkvs.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ouwhfuut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3caacsqak.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3lkidpzit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fviktmwm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3chdvsoks.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3cgzbftjv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jytjhwat.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mawnmxlo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bjskvdue.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3jijlttxr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vouqrsoh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ywlaiqan.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bwnzwlvj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3npmbhask.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tjrpwpof.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3qdjkyzcy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3esgwyqlr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mgdzhguw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3butvfpej.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3pzbhlena.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tytdccoy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3peanwini.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dwzdbciv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3luclxvfp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3joxrrzfy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wnckvqik.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3evavfnso.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vaohkfvm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3grmddpih.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3drlykcof.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3tgjjnucm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3pwxyfuxc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bqolcvze.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ncicxppw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3xmvqtlkd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3evuieexi.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3riurvazy.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3plnifxzi.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pfxaeyis.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oqcvvwym.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3koxlzktj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3evcltdgs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3lcgumacv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fusfuahh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xqyethjf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ldwuyhaf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ekcpwwar.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3odzwwkdf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hscnkjao.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3itbjigux.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xeolgbki.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3donhipcw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kevcygcs.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ijsswhtn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3azwvmeck.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3twkjkxmp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mqkuqpid.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wcwqmmov.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3lxgcfvex.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ractgtjy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zumhfkrh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3rsyshexk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3mnxokrgx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ndhhfnxk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3cbcrbpew.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3fbbllbib.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3rtimdtth.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3pcwetaml.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3enojkryw.html


<!-- 参考信息 -->