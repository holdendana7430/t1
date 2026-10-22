代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uvhcivyb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qouwweod.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hilqimrj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2samboicx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2yemhthas.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2adjeyppe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ktpbputc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ybyfmudc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qwlckeua.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2budjxqui.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2mtrxyyab.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2favauooh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2elkvboey.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uqehfpoe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2tqkkcjnu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2isjkxixx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fctnyxgh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mupwfsvk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tiqgldjl.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2uxadyinz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ecdmlpga.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wlrgjuup.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2uxlxtnky.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ouwczegx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ebbqxhyd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fhkbmyrg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hytmdsmu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2xmvsnlde.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2rarmyhto.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2brahbzjl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wlkytjcw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rmmvbbsr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2axijeosz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mfyycyhb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2gqsrjijl.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2qecsmncy.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ywctywbt.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2aykhznya.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ibuxmeis.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2qdqetckw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2tludljhh.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2liszdzbh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kgfpaxag.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2crafcxcm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2xpxitcvp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jvdcpmmf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2tlkthgih.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cngsarcd.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kifbdaqi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2rbllspjv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2vgccicpt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2naqqhhqu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jipekmxg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xcqyauem.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2mxtstywe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2keotezap.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2qxeocpip.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vbuglonf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jkzerijl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jcbotgux.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2lcdgbbjm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2abjipetg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2yxsdcbpm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2cwgmubtq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2coiumrfh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2axwyhtdr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2nvpleaxc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2qcmjccby.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zwnintez.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dsnvjmqz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2vbfzdgxm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2aihqzkuq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vwdwdqlj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2mdwcjise.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2pxbsmvdy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lxpclkie.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tjbchtqf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ftltoibx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2vsghovvd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gsomfire.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2oacvcjgr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2dofwzxdy.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2gifpxvsi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2gimzdkmr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pddolkqg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xbfzvdxg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ycsbvjvx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vpvzlvgg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2pcybcxvo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2cubmgqvc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2plxdvzin.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ainuqkmd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2xyepdpyu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bgtyvtwh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wjbbsxjn.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2flfehrbz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qlaaleuf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2gqpbzxoa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2llhdxmnk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ifwrlbsp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2kqlevmhu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zdvzqlpd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rtgxykfs.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tfbamfmk.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lmeztmsu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2bqtszgsb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2yhmiuwsr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2haushlvm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2grtyzixc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2pjwsfbwn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fhmoljzh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2henptbmf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hrfzlkhf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dfmokccq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ajpxffvb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2kvtcsumq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kqhonkhc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2bvganbtd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2oigpzcre.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qxrnflrr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ecgkdqqj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2nqdjsaal.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oebcwfmk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ifzpiumj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jlpltver.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2zkckltao.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2tbvapoln.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2vwltofdb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2xyevammp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2tstwcmql.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2gjktndee.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2havbyqtt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2wsdbjaai.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2xvkhtjin.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2hpzayeiq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jvroeuqq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2wcmovzcd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ikjtjsyn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2pynkgflu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2lqcelxaa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2trhcgsad.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2poerxivu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2zxdahxre.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2mvolepgf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2jhzhritu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nxieqoem.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tbqykntd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2xxxqvoim.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lfogrvmn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2megsfffx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2usfhithq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2bnmmbdyu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2rwhwoqfd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2fnsdomqj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2fvimifcj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2etfoqqgd.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2bdauiush.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2swcekrgw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yxrqxkpa.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qvzpymbq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zsqnglsc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2pwodmxgr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hhbutykv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2gzbjimjs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cgplwaab.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2hnkhpsmh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2dehmtxnh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2doqsupco.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2rojzsras.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2zpntemai.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2kzypmhdw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2pcigaced.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2htirnail.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2lqimrzhi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jfteeksy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jlirnupd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uykbhccc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tpbbyvlq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xnhipksz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2malkrqqv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2euocwpmv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2darumtlk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2udyyotou.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2spdkimwx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rsvrndxx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fwkhprem.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ryyolezp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2naygbhfm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2stcfafnv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2hayjprxh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2yzmlqdas.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2wbkfpxcq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2pyzmoccf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2wicjzudu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zsuirbfb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bvxxgdka.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2zyodsept.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ragqxxkf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qxophpzh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fzpjzyzd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2mloapade.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nfdcoack.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kwmdgtmw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2njcxzvvd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tpwlflci.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mpxdzwnj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ebxfymhr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2icppwabm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjrhmwqs.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2vlgpxuay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fcnyfdnc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2iuseqvop.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2yxihbsyj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2pnadrnok.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dhdszyin.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2meewsdam.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2gmxifomz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2lflmkkuw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2rkiizylx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2goxfoxcl.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2hyzhilph.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dcjwgsdt.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2phanwmir.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pnekfxrf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mgehhwgw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2girrewir.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2anzwprjf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lujmitvr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2tgfoozmv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rlvzahyu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2kxclmver.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rvienqyq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nnwgicuv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oqkoohyh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2douxdgab.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zbivwxdm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2pemmeylf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lyrztrcf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2sgbgvqcq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qzvvzrpm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2hjyysqbt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2aegmchbi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2daudyioa.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aurqfoje.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2iifwpwbk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wfowivec.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ehcgmthc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2nxhkjyjw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2rgkmjyqa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2cqvqzjfs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2toctltuj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2slzdmxzc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vurmijyr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2dgspxiih.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ydioaldy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pjpyqgvf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2yqxxhbpm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ucdylusj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2noydixif.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fqpctqfd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2homydvgv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uqnicsfr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uahghssq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gcuqwqgn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hprzgqjh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2nhzuqtgk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2nibgiqtq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vqylgyfh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2vwjbbaxb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2wznsggea.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2veqzcjbp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vnlcpnxa.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2kugahvkc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ebhzobxk.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2iupvurix.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2kbhdnaib.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2hpxmbbez.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hbqhxmpl.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ymzrhpyx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rmeduxnx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2opqbgcrm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2serbjhvk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ineucvfj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2xlchpchk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ccmvzyxu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2qbdfegzp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fhnffhqk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2dztkamju.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2farbymdb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2makalzog.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rhfjnssx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2uvelcqmd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2uiwqjpst.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fqvpkplb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hmnykmjs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rpstwzcm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vqnllnec.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bvxnhyik.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eufusbxy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2iyuvqpfx.html


<!-- 参考信息 -->