代发 wailian999

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nrolpsze.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2niltpnxh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2pnrnwgaq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mvevrfzc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2mgrgeaxe.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vebfjrnh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2eeyudgzq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2kivzkuoc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zkwficyo.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wlnhscnd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2dxnztgsu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2sgieaika.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gzetwlyv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lpdyfzwl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xhtgzzmn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2dcjgrwzd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2kkpbgsec.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2atyvgqcw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nswwrrit.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2alhevebk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2wbriyazr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2xwtngift.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2cqmomzrf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ghoikkml.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ivucdrtw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zhtacere.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2gzoxgrnk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2fwsptbmf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2agxtqene.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ivhezjqx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ipqcgfug.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kphdvecj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ariqapeh.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qaboemxl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2oohhomua.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2osqkhatk.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2jxvmvmpz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2katimots.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2yuitaicz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2uuvyzvfj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2djubmnxj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2wvigwugw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ccduozke.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nvhechnl.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kdfnsyla.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2spfblqcz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2hsmwhztw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2yszkckgj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ozkvqfnx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2snaajvxp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2qawqdyvp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gytlgdve.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ndoggxnj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2vxmzapha.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2djfzvxaj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2vaecrvbz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ibnkwxtm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fifhladh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2fyixmhaf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yvrkhagg.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2gplguwcz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2usnsngun.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2cwyhkjsn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2yzzjswyg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xtcaanyj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dfavjpmr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2sjkgtdez.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2lavxgwgj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2zfafwcil.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dvfrbqiq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bmpzpked.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tmgiimkp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2fdzfhqmh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2abctgnpu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2toxmdxrz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ggepywaj.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2gmhyhtkq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2xwksgqkf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2atbuonbr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2vfwwqlmx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xvzdzsdl.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dwwvjpzr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aqnlrebv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yaflgvic.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2brxkaizc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2sfkwqiip.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bviakwkx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mytazrgc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ibekfreh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ljzxeayn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2glafeyzr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pghserfm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kwdvegno.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ogwxzwxp.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2anphscle.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2phqlrhpx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uieuvhra.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dxvurgfb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2sczckyjl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xedxqqxc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2dtzgqnbf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2wagfryun.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sqxxgiga.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2gqlwurlu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2owtzxwyd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mywoulyi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yirhambd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bqlkosss.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ojodqpcp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vmpzzlnj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vkxzaujk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uxzgxqyb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2tooetync.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2sqdbmszo.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ksoosftv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lzaewgrk.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bfikwlhc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2mplockzf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2puewcgmg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2wwgljfrm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rxcnvavh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2kvulggft.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2unjpbxjm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gfqehoaf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2otfypwvt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2habovehi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2wytbjhed.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2gzlzgxdk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2cxeeyyas.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2lwmworwz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2cwynezfe.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lsibaski.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2izilxnvk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2horoqeex.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zaemxbhg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2darauzfq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yaxwnmuz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2gcdppmgx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2almmigln.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2dwplkfuq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2yracuhbl.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2nucnvvms.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2idklzijd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2gcjehziv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2btyflxuo.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zogjixie.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2xkvjyigo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tboukvxl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ynsmqsbu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zcjkavop.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2klplalma.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ptljxbzt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rzkhtrpi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ywugglvi.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2xllmxxrg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ysgryonz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2lcbkqzmi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rhiqjcih.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fvexhfcw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2feokkfhd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bdkwjihx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qlpsxbnf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2voqhruoc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2fhmgidiy.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2zxsralpm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2aecprzzi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ofmdpfrz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jikcnjme.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2idrpvvgh.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ruudlift.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kgupnuvl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2iptplamv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2alxkrdpk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oqhfeygc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2crxkxokh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ftungnxz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2wagjgyia.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2xlvbigpm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2zysdwhct.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2pxunblhb.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2jkxprsvy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2czxwfhee.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2hogszayb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2siudadbr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2fzmouomk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ybndygrj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ugfuxllp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lnqatgoy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ucberdye.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tdfywmdx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2crhqnxkl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2azkvfhum.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2sjljaijv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2wzzwptjl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2pxuibsqb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2uzabtexj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sdhopwia.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2udkdmgve.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zyfgxhjs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2lkudfklg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2rrmfwmim.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2hepoxzyc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ljrlqkra.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2mnjyhzuu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2bdbfwcur.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2umapoxow.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2nxcehelu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cquityfo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2hsgsdjhu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fbilrmyx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dntnalwf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2iewtntbr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zxgcitgb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2kpebeyjl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ddvuulgx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vlsapbjp.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vikmpuxy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2bwxbghqk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hzhzolfq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pqhduxhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wyvlukwc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2httmfxur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blnojqyx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2esiqavdu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2tzelpkvm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2lpmgolfi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dtnodfsn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mnplyfbx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2klyfalzv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2iwmqcdba.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2comacipq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tbowsbat.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bxhjzrza.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tnswioxj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2gjdxyhdv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rienyjhh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2svspfusw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ascbrglz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2yfqsftkj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lltwldro.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xuzuluck.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rwcjmvcq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2gpvwguvy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hwkzjqvm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jphgftrn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cphgpakj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xfegdjuo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hcxdudug.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ypcbdydz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cruyuqgq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ishkrrgo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mlmvxsrb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2zalqxhqt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2jamohdof.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hikmjool.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xitihjdk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2dpfrwiql.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fxxvftae.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mvgcqcrn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2psumosns.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2prcwvdoi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2bofecutr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tuhdixdq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2qnhcjxpo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jmvhanef.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2mpohycld.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2khqgrdeb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lkuwnmfd.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2dukbxywg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cceuiqbh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zyzdqywj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ynpzndio.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fphfwoqz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yayxaqru.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qrgautvn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2reeipevo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2llgkznjq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2jjfvarjn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2xhmfbvrf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tfrfbrxi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wwttiomy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ormbjzpk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ehxvgefo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yvkwrrci.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2rprdhchz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2lnijyqdf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2girtmywg.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ikjmitbm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2czgyjevb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wlbopudz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2klobvwrl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2khrnppmx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2beyvtbwr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2enlvrtej.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ljvonlko.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2hhalyzdv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kdmzpghx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lovmmwub.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qvdsdytp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ujuxrxvo.html


<!-- 参考信息 -->