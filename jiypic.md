代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mgihdghn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3cunsjblq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vzfysiol.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cupgpmft.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3rdbykhik.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dsfunqcp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3efcouupw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3gycwdync.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3wyrnaoey.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3axwkkyuk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3hziwjbyu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3spjxdeen.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wapvvkof.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3flaqcopn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3edhhdulf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3fgwwmxhz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mkkqycqk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ibkbsnrs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hmomichf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gjpbdxld.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sntwmclt.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3awivmxgw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3logzugev.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vobcqaqd.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3qtfwhdyo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eikdxtul.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3nruzbppw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3rpvthxuj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3mumvolur.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ytvvolhg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pajawlur.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gniohkwu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tnpbvslo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ayojlkzn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ujzhahmu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3orlgjcov.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3faakoqhz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3tdvsijcp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3cahngiak.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3dshkgbry.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3qazklnnn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ypszrphy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ftihotqo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3foinnnxh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ppxmtfrr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kcdbfweo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ypytsawn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3aydyhnsg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wgdmjvng.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3sqqavyhv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3pruoatfy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3dhnulnmz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bmqiavam.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ahdzmaqq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3tucjtaoa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3teeoiump.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3yqvnmtdz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dlmglqmh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lscreqkh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ecxujzfz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ugnlryni.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3qnhayklc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3lkatnfsf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3arezkncj.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3lzbxxzoh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3liqiobye.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3grskzwjh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3nlfmdydj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3drtuvtmy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3heboqatv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eueivfrq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3btrvtatn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pkfwrxcx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3bcxhuisw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3gmaxrhae.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pujcupiz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rgbehikc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cnkxznqh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3lfpwibqc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pssmtfrz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xuezrqmf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3donkckzj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3oafchprr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3uynebgsr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yuyovozd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dfbomjag.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ceysbvdc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aifkrkbg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3wdlguwjs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3edvggaxc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ypetzgyb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ujptfilq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3awlkbkmf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kkiqpdlj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3psuyzotf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wgtmfevd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vxhekxkg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qizlrcba.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3katgoymv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ynauehik.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3sebylvlq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jalomwfi.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ezwtviln.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ljsyiiua.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3iavsefmh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ugaguide.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3xbeuyzrk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ycccyjmc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3bxezejhl.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3uaindigg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ulindgjs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hpbzobcl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3voonewow.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3acsbzavd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ztruitxz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3fsgzrjfb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3nlfiyeol.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3gvymcrgp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vffxskdy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wkhfneyv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3xfmomzor.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3jniqsqry.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pkjxcxpj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dpzucqot.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jgqeavjj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3xliwexut.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ewwcsmhd.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ppcfemyo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3hpkfqote.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3kvymntdx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3pnqbxhyx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3suhcgmuz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ktqnbxwv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3azxfsgbd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3akxewsfi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vzurzhgu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3jdtkbjze.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3behlqgcr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3pehrgomq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3hapgyedj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gtvzftyw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ihpysjiv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3cwpfppgd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3xhiyzoob.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3boukwsfj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qtpojjav.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qgrlmhoz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3agxirgqc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ljrrzwzw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3anjpojkd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3bqrffnjk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3unltoisr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3krhliotr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3wcxmlwga.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3eugqkgzt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3yvxuktir.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3wmpntwtq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3svzzhrek.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nlluduad.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fwlfcgzq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fuxfwpet.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jpjjamun.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3paihpyam.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3nydpkypq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rjtcpfot.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3lezbwyzc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hoibicwq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3uuglbtbu.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jfnsafft.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3vztfcnrj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3oenfiuxo.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ssdmqmhq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3pxiygndh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3xshswzlz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3tdsxjbkj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3haimwzny.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pejpjili.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3rkcwrquy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mdopvedf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3rrhxlalx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3xlllqfwa.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3girjeydr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hsbdlfsr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hxgxkuur.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ycwqgsdu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zycmodeq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3xncmvqgu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3gmrvoazl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tdhhticb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3hkauzcry.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3nsfhcrdp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3gjovjipu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3oaplqade.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kzwrwqnw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vyuvuwfm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3adczigvl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3nehucjkb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iblkcmyq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3litslkik.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3gypqubxw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ybhwjgph.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rvvvydly.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3koispnkp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3euegnxwo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mjnqfgvk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3noucziep.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3euavcjge.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ravzdrqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hpmwtbkc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3yaurolgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3heqltcrn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mekfcisg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ojdoyroi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gpcnkuxt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xfrhxndj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3pyjtnhcq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3lnwosfen.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3dwskvfmc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3powljbsm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zwytsziu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3pqknnrbx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jvtrurdw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ffebgfns.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gyxvouuc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eyzuddod.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xvdiuzqf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xsjqtdad.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ehiswvvd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3mttxssjf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lyrwglnm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bqlgiadb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ybnkdgmq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jbzprevh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ugqwavcb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pkmllaqa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3uqgvrdpb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3xaktfcrz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3wgtgnufk.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3qgzdgzuo.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ezqwnanh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3hbfjiuos.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3zdqyxeci.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ocahfrua.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3svvcgwes.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3tyktdkqx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eqzzrkij.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bkajbohl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3jryikkay.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3qosuxhdo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3zikqcznn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jafzyyrv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ktsvyuvo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hyebitfw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3zermkpog.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jmwmypuk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rzzspfpo.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ctqoazbc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zpftuavt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gtaedzqw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hysiyzlw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ryoghocv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mhcvgmpw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zlziggsk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dnmfsvrn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uodomnjl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jcsjhzkw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3cejkdayt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yiallkyw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3niafnzzk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3pidotqec.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ouiveodh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iggehruz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3stdofovx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3dzqmgcaz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3rlrmscby.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ypfkmhgs.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3yammfqqc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3plxaywyx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hdpnrbyf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kljztlka.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3tythzkka.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cbansrqb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pxibcaeu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3jbqnmvjz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3vovmnvrg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bjwjdpld.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3juebabvv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ugdksjtb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bbenxfjf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3xiaehpbo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ckoxxetl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lgaktpac.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ozgusgly.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ovjpgoih.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3cykoykcs.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nrnyzoow.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dfkpnfmo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kyffknng.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fgqydxix.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3skmbixaq.html


<!-- 参考信息 -->