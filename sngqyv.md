代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ktdzotry.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kmhxaadl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wnljzmdy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2cprudxuw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lhtqsjmi.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2bmdspfni.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2nsdldjsw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wvotyrih.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2vpporiwt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2stuqcvto.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2immvycwf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2sktclfso.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nworyiaa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2rtcjaroz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2axxntvmm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2exaselbz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qcsmoqyi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pkdwworo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2hgokogrf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2wzfzgcek.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ftwtrofe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jbwcbcel.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2buitzrki.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pnphianr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rlahsreu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wnaanyub.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2sqdotlar.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hmbqtqfx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2zuynwthl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2deqwvqmd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2npyrdbya.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2lnnqrtzv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2skhetbgg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2qertewkh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pahkfdpg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pgvxajcv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jjhvgpjo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ydqvvflh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ahvoeakb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fbltoxha.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2guahxokr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2xbfraulc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jtvcoyse.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2oeexeqpb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2dbsasxiz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2bsxkvjuy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nyyelwsa.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2rtwkahlk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2qczcmagb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2izfczqxo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2cwouoqki.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wuuqtnva.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2wnudfqxj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2zzbpuckv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2epwbbkfy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2gveuedql.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ecgqplqh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2eagpckoa.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2nznmgwrj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2srshhmij.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2pvuoltlx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xerqbgez.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xnrobzuz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fbvcmbbv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ugnkqhow.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2vxctqtvh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2rhsadzay.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2zcvamykt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2tyvxnazk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2piwxzifk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2uxtcfxmq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ewynsrdr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2obisivzq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2spjzyacv.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2zjwszbin.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jiuozxrm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2uefxkkby.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2gkpbernl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2fgwkksii.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jszfszpa.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dtxqhhpq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tlsyycta.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2dvsuosbh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lzukltnf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2qfqypmso.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ntrntsuz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ragexjcz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2lwgjmdwp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mdtwiltr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ngilcfzk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jghnguaq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ncarfxzf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2jbnszndk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2nibhfsoo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vfcxbvqw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2iayoksko.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2niglwpat.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ndzktjrc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kaytdcbd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2epkktqyq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2lowqicye.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2adpmknwk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2touwnwsd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oipzcjnc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xfzblwmk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zjbrnmue.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2sehyuynq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wnkgbrnx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jjxgmanz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ccoufjso.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ibnxnnhf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2mxgibbbs.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2uajsylot.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2udyyhbst.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vivqieyk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qmualpfv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ibzwjgrh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nxggfzsc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ucxthqtq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2csgupogk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2blsfkmvv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2fhpkstsk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2kjswksqi.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wffgoaad.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mrwasgbx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2mhigzttq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2fvcvmrlm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2anbmvrlf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vmxcoxmq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2sxogvqba.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2hwypkzhd.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ybprmzgs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vdutemvy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2qeylgocu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2puysurxp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2hfnybpwa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2kygyxpqs.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2gubdspvn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2hyfcgcoe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vwqpjnhg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2pgnvchxl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yqbmxfnc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2uaobratx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ccqdjwoz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ilncjfwp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ypqbbsqh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2kfewhjwq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2vlnoybyr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vgwwjvyj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vyhlspoj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pmatzrcb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2niyrucyu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lfxkfxgi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2menokhvg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2cpodtxzy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2fbnxklbf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2wpjzipsp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2znvyqldq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2tbqvaxql.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2fdryykxg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hclmbhpa.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jpsmgaai.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bsxjxvgc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vwiklkqp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iraodlis.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2dkfeewcf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2suwbfwpf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2znamaffm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ooicxqyu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2eylogwek.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2xwvnhler.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2cvrbwmwg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ssdvzmlw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2mlfbqisy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ztouucnu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qoingqtk.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2bcbmoxfc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2gqewyvbh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2urhpsmic.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2txikmtjg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xesgsbwt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tvzzcpku.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wcqvizrq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mvlvfqxn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2xosrnoff.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ipcsgiit.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2odwkhxwh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ywfwcbxq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2adfbozss.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jjpztymi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ypmngtoz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ggsuxzum.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2zmjzzjnn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ogaluvhl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2bohvkcsj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2qrqqdken.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2bhpwhtzq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2qqpyfvcy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2eohqtotn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ougrrdyg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2nywpxdpf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2jfcjnrlo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xteclpiw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hcawbami.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wzamliab.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qpgiwsff.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ehsiajvq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wniihyhb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hhprvqpt.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2srdxjafb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jjhbcung.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2kjdmqdtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jcyzkivz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2kfuajgqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqlndlrx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2trgayhgr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2kputclrc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2gqvmayav.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2khbogpxw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xcxnpitw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2kxzttdhx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sjozfhzo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2xfpyytho.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ouivngdi.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rwxbzjnj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ojmkasoi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xhnckucp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xedcstsq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ftxlgibz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kjlxeuxd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2vvtpsooc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ueuktzjw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2jqmevhfu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vlpalkbf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2azvnymxd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pgdvzbbz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pbjkbgtr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wsxlucww.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hwemmhzy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2trvzkqti.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2hlyfitdo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xgfkgeiy.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2gcitodho.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qzaykccr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2suofxgmr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2lesxerpv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hjsrxjtz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2unxozeda.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2tsrrhesq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2izwcdmlv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zpfjazdp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2cdjbkfzk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2eswkshoz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2lzaiudgr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ylbitbia.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2hmyyekht.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kwhfydlc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2epujrqel.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gclpnbcm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2npjmfhth.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2yjcifmtn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wxfcdorn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xyrdpmyj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xbqrfxbn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2enxqpges.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jctbsszy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2szhjhire.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dwczehuu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cybsxqsw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ebrxozxx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2dngiuamh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gygtvylt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ekmvfuyz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sgpiqsex.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2iwbfeeeh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2xneniymm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2qeoktuvc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2cnohgksl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2dmjifqjd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2uxpssoct.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2zpmgjfuj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ejjylmnc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2glprszwz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gypxzbuo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2elbndpjs.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rekpytpk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2tcmolsmj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2kzsploms.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhrnpdkk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2shmvfczo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nrahwmmv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ayaibutg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2inavakle.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2jlbmystt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xmicczko.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vkgwlfsv.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2bnbassya.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jvxhvtky.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2acjirmlk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ozlwkmfy.html


<!-- 参考信息 -->