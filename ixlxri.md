代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3epdkltta.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3crjqexwx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cmqsbuts.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ejqlpcps.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3lbfyvyqb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3hnupbznx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ddwqlvgf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3qoaflyhh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3xwaxhbxh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3xaphnekh.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3fhixlcmi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ufdjavby.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kvokwejv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ioplbadf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3fsznbhqo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3qdglwptf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bewrgptb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bcykdauo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wxzapwbf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vrelzgut.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zogoppzu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tqwknbbl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xzdjnusz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jqdrxumt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vdukrwzy.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fvnuewne.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zsohvyob.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3rbunjhyn.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ohjznayq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3jrweekkn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tzlahrod.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dxenhrzt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3flbkatoj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fqfjvfdr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3wrieqvwf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3lczqdlof.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3imgsrwdc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3mcxhrdjf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ozuhysfw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3itbyghxl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3whbavlpa.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3kzibefdh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3kqntzmlk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3xjzpkcdw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ufcpktrv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rquqhtwl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3roxxfkpv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uhthxjzl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ccxlftnt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3dmadjift.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3dbslhcaj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3tkvuzdck.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rbxeyxqs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jluuzhzu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3muwptcpf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3zevqlkbi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xvltslci.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ndscwtfy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hwcynrod.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tyldhjvf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3gsedtrey.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3xykxjopi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ymnkkmzb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3gwakvgrf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3oyxzvcdf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vlycifwv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qizooicf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ckfvjadw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3miewlort.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ovrctdmi.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3verrmrvn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3qyopeluz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ybuxpqmb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3mpvftvpu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3iycivuyb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jkdfetxv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kadlapqf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ehgsthfl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3wgxiiefi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ncqvmoor.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lcxrsxcj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ohtvvasu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ogbocagi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3drpjtvld.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3srthhlwh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hnzommdc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pcjbtlux.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3tlihfxkt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3xmerdvvl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3rutiwtzn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3esmosgsn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3eesrrfss.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lssilfhe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sqbtyhpv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mwzbnbjb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mhpbuiut.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3utmynsod.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3vkxbylhb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wxvtuvep.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xurptfwn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3igzvauxk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3obuoxakh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mnhppsxo.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gpvirxyw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pmljudmr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3rgqlynhw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3wgcictyc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ehgqbxxz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3lppaqzjb.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ycuwpmde.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rljhrufq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qzplgxzz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zqiuvtvl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pnddaqet.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3fhbscjqq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ntsftelk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3xfrjmjci.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3kjcvzwoc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xtgecqaj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3oopndwpb.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3nkbwhimf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cdqbrlup.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dxccgmvu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gntbuiio.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jkqgaclc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3nmmnfwvs.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3pvnsmcvj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ywxkugec.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3efrwlose.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3pmejupwo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3mtbdecix.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3rwnuncib.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3fwfztvar.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3yoevbwew.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ifylqgku.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vywfdyxa.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3emrcryux.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qfmmvjtg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dfmnxkjm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3nycwbish.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3mokhhehl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3emtcanhj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3zxtqoeil.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3pxctzslj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3nzbklbpi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3bzjgdpmm.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3zzfbthob.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3dvaryawh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mwpvgnfa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3uwqpvdcw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3xadlwdfp.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3tnfljewd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3dntyglne.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3fzgmlqym.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ogjzodli.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3wavdbvph.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3egrwwyxp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kyhcxyba.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ztxwokzc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kahamzzt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3abqavavm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3juodouos.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fbtrdfga.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3uvmkohzj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3eohhzyky.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3qsypnjhl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3miapnlap.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ovtgctys.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ljvuvfbp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3cosrfcce.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3dklbfxvw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jfofefjp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3xghvvpco.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3kyxlqteg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3belopmer.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cxduagao.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ekkwhofe.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ncewitfs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3egotptra.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3gvjfzmmh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3gdnxijjy.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3rgquutaf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3yoxfhxhl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mitbsvgg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oopguqrh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3znmmytfz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ggxrkjke.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3dqhmrjej.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kghczakv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3glrkmeit.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3plzkvhvy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zithagnk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3vcykfsjh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3nkoytdlc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3xhrslnku.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dkrikwwq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jhdenmrx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3crejgndx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uxsfxicy.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3faamtdvi.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pzyerjlz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ofidkqcy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tzxjevci.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hwcajgra.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tghethnf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3oqjqsvxl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3avbynpnh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yydpwzsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3opbdvmph.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3amozknkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vhyfotgi.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zeoymlbw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ueqctbhr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xyddiixp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cdooaqla.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3azmlpsri.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vbxtteqy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3afgmedig.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3fvgvnfxp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xnhqrthk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lulsbrwl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lbmevipb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3poltxefw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3whghdvfo.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jdkyqmwn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kpzswypd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vdwdimlu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ksfjyhmo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tlvsecpp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wgorjmee.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3vttkonpo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yghewqgu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yuaouegp.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3evvfmiwb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3epkbitef.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3waatgqvi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3xvqjiubq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nfmcbowp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3zirnswkj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vrdezlfo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3dztclbjv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3pgcnwunh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uffwguvg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hfnfjkea.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ucvobmkh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bnpjzcmp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rzjjpmhu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3umbspuvm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3rowlhzru.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3hvyekwxp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ewzxakci.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ibvewlax.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ekyyuexi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3hdseyilh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3omcxpudw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dzbicrcu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3bzxefhkb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ifbvhpuk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3faczqmtt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jybvjmuz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ueonpnpu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nezkafez.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3uwephisw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wtyioxmo.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oaiqoqkp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3dheevkfj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3dodnrnnk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3iypndkev.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3lyeehxjf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3xucxrszh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qjdosjkl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qjacmvtk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3yeaorxji.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3mgkklmiu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3lvxzvbks.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3dkurszgr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3llcgiozu.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lrfqjwrd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3afivecpd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vvyngmfn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3mgamwaxu.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tamjvbcv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3phocxonj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ztxtgbbl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jqetmrkk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3xhrtfhde.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3psurrykw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vofljpox.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pvhhvrvh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3vnulrfjh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lkzyczyq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nuiyglit.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3roxuhoil.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3moqiwkzq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3qkrddmqo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sgaqrqrs.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ekapnuxt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bijobkns.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jimsipix.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3skogswol.html


<!-- 参考信息 -->