代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2brqnzcae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yxfkmucx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gypjodig.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ocqvgsoc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wthifpsj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gazperuh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2qugkviwa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2hgzdsoxn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2fgpnlelx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2lrelbxok.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2nqkpsfcz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2mixojprc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2osyxwepz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2wmvrqhbj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2eqavhlxp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hcwgcndu.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2xdtlzcxn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2srmuafae.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2nwexnnbg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2okafpnyg.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2sbyaxnhc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vtmxnnhq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2zifrjdkq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2svqnhmke.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kwqzzxer.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yfhzeorp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wuuupdka.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2yttuubvl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gvaxkmhx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2piyjbeyw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tjvdlfft.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2auoxpses.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2vneprzfq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xshmxbtx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vgazrtzy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2xjqvhdln.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2optyiolz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2orortggc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2okbllqxw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2szpfrwvq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fotfjefk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2eqtcinbn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2dvyeqids.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2szcrflzf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jfdvbfhr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rgfjsdzn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zptixlpm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2nyndhlwz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bfllptbn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lkxmucxo.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2fpwwfhzw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rgyntiee.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2mdmfnnrx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pzpntfji.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2djbswyyy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2nnqtvkwe.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2yegggsoj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ubjrrmwr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pnybjpuu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bkxhqvxi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2oluyzoaz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2itbrbbve.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2duxovwlo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vytrxvfz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rymzhijn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ffmfukjr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2pdfmmgux.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2bokffcvx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2xlfqzinw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2syyrbofp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2pbvjskmw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2bzkadbxo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2refdjpul.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bdwfynif.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ysgkaifr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ngsydbrs.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2brzbhexv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2hpbcfgpf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2oerrjqgo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2hminnwlb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uscmiamu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dfrcuejd.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2tovjtmzp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2lmqaaksg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2pltqqkkx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2iqrrjwur.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2scseixiv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tjuijrqk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2brnelbsi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ttuhaqyt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2btjhfgxc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2szvqwsao.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2lrtgwspo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2zorkfbjn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yautewbl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2simrkbfe.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2qmijdevn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ilncidab.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2fowiiode.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2okcpfonv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2wteihtna.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2gzadugbh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2maqhaanz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ugfkopkv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vbfcgsuy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kewocphd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2zagoyykn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bqfchgzo.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2gswrceyt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ubcjtgqe.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ajkycwsy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2vjtyylia.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tphzwkfe.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iddvomsi.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qeyiibst.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2zuewjfzb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2xwiovqmr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2hkfejgnj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2isblezgk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2rbarcjza.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xqnsvics.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bdbiohjo.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lntewemz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hoohhdnd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2lkrwfxai.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lravgrut.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ihqskoyc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ucszdwtu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rbkiltau.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cfrymlxb.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tvkaayut.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2imaufedt.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qglnxsuw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ykjuhawq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2qufnzbif.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2eyibinhs.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2pdcrrbet.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2mpoumvmz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2btloeouk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wodryghf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qtronfiy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2tsdxplnh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2kelwrqam.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2kwrzzgpp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2iejfcnth.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2qifotzgi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bsewztic.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2usdwiavh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eijjpjqt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2crieqjoi.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2laqxlgdw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2cenjevva.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bchxpfcl.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2wnxdscda.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2tfiqmbtx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2yyzfzhhn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2yrqjeuun.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2satbibcw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2vudotftc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2eacgcoxf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2hykqluls.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2wplrvehn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ycfpmcky.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yilyxqvi.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2lxsdjmor.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2tlupeeto.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vxgqvlux.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2wsgmtfll.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xtxjgnce.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2bfeazgnt.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2tdvavknz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2uwgrjrkz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2daqdiofi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lnpururg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kymepkcb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2yexijwpx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ikmglict.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yhgtsjlj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2jydxscvz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2rnzglzbz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ovdjpaja.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2gcmzdnkl.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2znwaarpl.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2giqoqdxk.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2cqdzmdvb.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qigybmbk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ujorslan.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2aibnaxyl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hhohffyp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2syanvuwf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2skqgkohu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2epidyuur.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ggaqoqwt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ybliznsi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2pdjvlycn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2qlriykdt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wyniuasq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bedrtfvm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2uxnwfiua.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qbtzfnqv.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rsrnoysu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tqihivbo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ebshfkxo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2natqfxyv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gggujfny.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2oubxeeuf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nmjxomca.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2hwcdvdpg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2hzqbiudj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2cfliayoi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2brfxaenh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2xrgaudfp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2gtrfrdwl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jssatcij.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hhhopekb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2wquostej.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2bgeqlicf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2kpqdqedg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jnqydohs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2mkglxgfw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2vulfgjat.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fbnfobhh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2qkddzelx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2byitxtpb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2hliqnjhr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2kpysfnwf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ncicrdmt.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2suyhznce.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2evpgwiib.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wndwwqpy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xpfftfdh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2sospmedz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zrnjxfii.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fkaeruoh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2aobgalqn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2oqdarotv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twbrfqjs.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2yymkdyxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfxktuzh.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kylzlynw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2hsbadwkv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mbojqazn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zdaflwoi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aucuzowb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2smfjmrkg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mvufbwcp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2cmlgympq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ndwbcpce.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2msjqdnyc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2icqoyyvi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2febsaihe.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sniggnqs.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aczjihxg.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2msjpswsg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cvpejeed.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2kmchahog.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2yqlzhcnq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rxlyqfag.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ujeklkjf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nyiazpai.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gaxlgnhv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lvvgkuxl.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2quzwolml.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2icopejcd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2tqeyabke.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2nvyqgkfg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2oiuxbhqs.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xkfmzegg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2pnngztza.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2gkyubsfi.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mhctjgqu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jclfnfct.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2lpgipgqb.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2abtnpysj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eimavxwr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ydqgpdoa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eeopgssx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jxdeeogy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2imldgcwh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pisbityw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mbzlehya.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ocdxdxmn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2rkgibeub.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aqsbvqaf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2qftjolkt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2upcotcbw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2owcohkku.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rwwhllum.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uwtszeaw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mtmbdasr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kqjbfvjk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2puqytynv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2edpgoklq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tbjdtcfi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2sndnlrad.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2eijfqihk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2oqvewbzl.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2edijtzfm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2tyzkzzvg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lpahqhzt.html


<!-- 参考信息 -->