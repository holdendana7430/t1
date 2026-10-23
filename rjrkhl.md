代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wztykyyh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qqwllmbk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xsfsmipn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3oxidhejj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jiyjyrhx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3nnxpsuun.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3nooroqow.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3pnsnippj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3srrjfuut.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3iklubzcn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gtmzedeo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3fuxfzjsu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zqvdrhsb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3yvzpswxk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3lbehpucx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zafgmfry.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3roieazoj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uvohmatt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3aywkiior.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3etrxjcyw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cwyeuyrr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uumvhhkt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ncydehrz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3phimcbro.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wqsfvwwp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ojmmvtuj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3aduwoxgg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jgleyjbh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ztsdlkdv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nhbxcxvf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3fdmpdrcy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3dtrypmjs.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3elwzeypx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3uymcumhv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3izlgrhqq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3azytmlzn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bcuztwse.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gvxvpxir.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3zfppypqo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wckmmath.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3psnckybn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3vkddcaqk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3mohcwecs.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3qpechwkc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3shjjhyxw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3dqtlhndw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ncfeblux.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3yrmtyesp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3xohnhfwp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tenexmkf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3eucobvpm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jutylvec.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wfaqenqh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3bhgenptn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3bqkipzdf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3xgaadntd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kijdrjam.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3izghkebs.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3bficfowx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3chqaesfe.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hjksmnqr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zbrnbdls.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3uanztkno.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qqjgqdor.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3mqzyzcbr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rstqiash.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3bewjcxft.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3mqigesgn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3yqyhyejb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ohzxulnf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hjimfgch.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3psbhnfjb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3lbibaudx.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3qzsqofsz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rxsvutyt.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sohquagx.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ywtylixg.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3rznahdjx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qibxgtdj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nvtbmgat.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fjhcvclh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nxfnrxsi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3tjjtnuuv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pyymxyaw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lfedmhqv.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3dswurifx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3tnztnrvb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gisaafyu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3lpoheysn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aqiphcof.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ybuxzkft.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gmkiqhnq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3wlkczsts.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3mfyjmpbf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xiuklvbl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3pbwwheln.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tyzedsks.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rbaqlkco.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3sfbfjcej.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fewlchni.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3djxotuqo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xplyxbyh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3blmmjaqk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fuoobwah.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3guiokyar.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3flbuqtqs.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3onjfemib.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ibqmaejv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nxcqhwzp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3iufwdzxj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3kgxtypej.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3itggqopf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rmdsvlnt.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3bytrvmzi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3egtlngyr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zgjcnyvr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qvamqlos.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3msabmyxf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3celtcnoh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ifuetnsc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3wlhzvtsu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3abfmazba.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ypwkkcjp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vuphkmrr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xhtwlwwj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zlxiyyok.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3evoszhqm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3teuvpslq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kakmfszu.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3iqgpgugv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3suuxdxtt.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3jvvdjxby.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3pvbtdabt.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3orqujjgl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3fsvyypuv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3zdtlatmn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yeakcaib.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3bpvjtjpj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3alvuceia.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rrefjnqe.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3fccujigo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3cwwfcroc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3stplyfxg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3wzawcphi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jzkazdch.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3pyonoxjx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3mxgmkjsz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3uhfxbrcn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zjaeqyef.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3kizxossd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ivlhhnuo.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mzrtyyck.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jojqfihm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kterjvic.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zztspkit.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3gzhttdnn.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3tdibdicw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3dhjxyfqu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3xfdrhflo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3jrvbsycf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3tzcutyxp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdldypno.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xnamfpcv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lbzzlvtv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jpwuknpv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3adjzlzbi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tsxrnlsm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3lovcixvy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3mtzedyre.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3cwddtylh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lagkzidt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3biemxpbw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3muaenvns.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3juhoqxma.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3stdfsfpb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kvlhpkve.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ncbyxvct.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3turfcwnl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bsnxrdch.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zzpeyyjz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3spyusqov.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hburhdkt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jvrujuuy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3xijzkhvp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3iotxuiuc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3qppocpuu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ypxyjwld.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mnykjqdp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3itxdxciq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qpwnddjn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3caieuubu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3jegjndko.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vzkgjfyq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3igkwvczn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3endekxdz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3yoltvkik.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3qvuistlx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gehdvilp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3spzgjsnq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3gxolplqo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3acuilpwo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3zmpawjqa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cwxwtmda.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3qemoeeif.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3hedhjzye.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3amlmwepu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xmxhnavu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ntspxzen.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3iyamoohl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3lukvqmsg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ckdfqmah.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3pvvfkjop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ilqbdvxx.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3rrpeyavb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldwjyczj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3llighiqq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3sknxzzbw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jabwnnuv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zwxbidza.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3iwtjjrhn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3kcfkswlg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3orkozqmg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ymftfppr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hjeaymmb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xdbkqdkz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kijcjxya.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3anmplfoj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3urbgwfos.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3stcaplpj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jbftfqxx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3rmwjxxqe.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wlwxshib.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3sovakpqo.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3guppzdxj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3cexwhjrx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gpkqggxp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jbfpfrxh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3furntbik.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fefuavvr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3lqqqrxkn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3eilkpqge.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zbogxkqr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3uykxgtml.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gsaqigto.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3cdmhldzr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3roagtmqr.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wdhbuemy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pdtqgpzu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3gqdjyisn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wrmzcuak.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qmdzqmmw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3dlqbohvf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qvyljnyr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3iormcwkw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gxizxkgr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3fwgytbxm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xewjiwyx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3mjwktkzg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kgyfmvnp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rumobtmk.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3haduhlxu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hyqnbgfn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rizhlsmy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kijsqohw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xmnedflt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3abwcgnjn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3baffbojf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3efenkvtd.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rybhfyxd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fnevhahm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3xqvvdiqv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xcebozrb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3mviycxtx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3lukdsrfs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3mhctpjzv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3poamwyfq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ckbziwhz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3rgyhtgpg.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3jtgjidsh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3zwfdvbom.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3uilfsugp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pmebzuqi.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zgioqnzg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rhrlckob.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3qmupbcyh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xpktrwwr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kslcqbdd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3xnxbinat.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hrobvvnc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ixvujgdw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gljyrevq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3eqyrtlkx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zqacfpvu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3uizbksix.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mtfacbpb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kjjoelgy.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3wuakjowe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3auakyfpb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ehfdgcmb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jbyrkwnk.html


<!-- 参考信息 -->