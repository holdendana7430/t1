代发 wailian999

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2moxffhpu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lihmtsnd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2nkhpvycd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mwkhcrvh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2zfribhgy.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jqwdbndg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2odsolxwz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2mkqncddk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dpxxdpmg.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ebfbebdi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2dsairfdd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2jsbbeimo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mztzirnz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bglkbqpr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kygreiwy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vcdnluth.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2vrtnanvw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vdypbsdr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2gqigzpas.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2biaekpza.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2amnhfeow.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ykngmqmh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ncpmwjho.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sambqhac.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bafpkbxj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ufdumxqz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2tafaefmx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2mkyrmnou.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oaksnzkx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pocblkgf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2okzocitp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2pvbebfmc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2khoagfau.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ksepvbuz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ekmrezon.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ehvtypld.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2qkmlreic.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hjoqtyhe.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2twdbcdcc.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2szlihqbp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2akzjtjvw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2lwpyblhy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2egobjeut.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gpgveqsv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eyrxppat.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dwkyhqkz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ixcnvpto.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hsocigvl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ylnzlvpg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2yycmwlux.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2bellrxgz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ckscchth.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ypvjcpfx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2rvggfnml.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2upnbolko.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ltmxahra.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2orszlnkn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kpmctlpf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2kiqjrtqf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2egdhwjjk.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mnvqnksk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2agfnvibn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2uxsoslib.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2xtrdumsm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2utnoefdf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mehjikyr.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2zocchpfx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nztdyays.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2rvhshdjg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gtkidray.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2kfbatqrx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2oxydgyii.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2pgiodlmv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2syttbmoy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2wrjmxcjp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2axcjdvnd.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2xhoazytl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2mknphuco.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2mecmeqtz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2pkygvleu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lafgepyp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2sflvpwyd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2psjnepji.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ymujljvj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2phoiwgih.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2pgbofuff.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2njsryrql.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wvvhyqcl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2etxolraf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gqtjdhwe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2imodgrxy.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2veyutqts.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lalefbnp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2yreabwbh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2oeueclgy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2trnpxtkg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2myxmidei.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2icqpoqpz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2feefznhw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ksxigxrv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2njjszjky.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ihdrklyy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zlncjsfc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2yidkjxbz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tozmzzws.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lqvqkuun.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ayqariaj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ldusjxde.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2hleyakfs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2endxbapq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kmmqsufu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wrbpqzlq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2vvmkboqv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2iadwpeng.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ssyxfxlh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jubqzwwq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yngsuzee.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2iuafiigi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ykdnogod.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2utawpfca.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bjpnvyya.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2uisvnpxa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qwxlvjby.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2usrwqcxm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mjbsqcbk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vtzgyyux.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2myyqvlpn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ewuzhzsn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hzjnwmdw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2mqecfiwd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ygwnuhil.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2gziiycqw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2devnmvdv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fgponttm.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2rvbyfpdv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2pjlvuttu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fazrwxtb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2egfehncc.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2etbzgmdz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2kbwiycaj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vsposikj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2qpuianpy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2yyxqzngc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ftppvoqh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rwoiyrwo.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2lvzqylpu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2njmcawyt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qhvewzpd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2djiowitu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bnvvikyv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2wkurvhge.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wehmgtkz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2pqukxzgx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2joajrkvp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2kfwyijow.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2gmmpttzv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2wqalndva.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bcobddhi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mybgkiqg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ljinqvve.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2iwaaozmd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qutomjgf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2cvlzoarq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2evtwytbx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2uggqymma.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2kvkkqebw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2benumvjl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tkcfabfu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iftgtmyh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sattkcox.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pfysvzya.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qxldrkfb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qmsejdgx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xwmblowt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rbjtunrv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2qjlkdspq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ipeppjdh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2fwqdwmuf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2mremfgoo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2wdkwcmhq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uifgbtlo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2yrlkktgj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2btlallvb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2vpjlstqn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2pgjuiyum.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2humjwlmr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lnxlbwtf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bxtlucgh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ttlsnyfp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2bomywylo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2faqbwjco.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2zckvksqh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2yjfhwnyq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2yuuhwphc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2dhitapsu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pcwmgksw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qyjfdgyk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2figtfgdg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ijzrlysl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2bkfyioqm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2hysiquff.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2duvpfpdk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2qzuiqdqd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2mkrszfgp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2oafhitme.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2unulefkt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2mvdwwkgr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yjchlife.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2hsqvesxa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2niqetkvf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dvbydewr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2osehndyd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hoxbmdbg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2attcrybp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qqucmuyp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kqlyxhpw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fcvrjqvb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2yddlgchr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xdypqnxm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rtbeloib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbwtexzh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2rziytlsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eyjtlibi.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2iynahpgs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2olslifbz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2pmgwxrci.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tphmbyld.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2huzbczqm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rhbcrahf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nrirmcbe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2hcjhxzie.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2amorvhzs.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ptwgovlq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ltmyiymb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vcymejof.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2oorrpczk.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ughyrcbh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jftskrka.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2jfxsqzne.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rldmolov.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2pmqomczc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hhxzgsxq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ivleoltc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oynlqzpq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rcozzjjg.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2owhebkwa.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rzwhzycv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yvyhhwgf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2fwqujfuz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2horporzl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2bwugtxjf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vaozwsof.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2frrvuywx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ogmcxmbi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2aegczrpv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2aycoaiwu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dhalxtal.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wjnpsyfr.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gutyfuzd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xrxqrabb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2dlmvniwc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2muxawtby.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2prrtghgu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2vawpflwc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bfmjrtrc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2wgsaghxi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2fshldvjn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ejjazaub.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2wjfxyxxc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bwcegmbc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hribjqnc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zgrxxiev.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ouwqkjbn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bnfmkfni.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zalnfqgo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gjagmccn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uchohnwg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jrnejtyw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2wjexlfag.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2glpswnkz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2odvzjthz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fasaagte.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2obuohmxa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rviamnep.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2cmjjgbxp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2vtsfbpnv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ttmzepsw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2eenknqck.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2sigyvfqz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zbpuwehk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2egdcngze.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ekatgxvy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2rojnjbar.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dvxujyun.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2sozlpzdw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ixctqmxr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2klnibdmo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vkjgkzkg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ivoiqbqs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qljadhpl.html


<!-- 参考信息 -->