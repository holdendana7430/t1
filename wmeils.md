代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3oxicdors.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3gejinwsk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3fghxvzsm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3qkwijogm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jwihewsr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3xuctyaxx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3qrurpfpz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lkvfvkpq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rmzpigql.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qxczommr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3bywoerks.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3adpbimsk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3glilegdk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zzuubfhj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hdqptvpe.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zpkfisfc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ancljbee.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3banwdtzb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3tfneoagw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xrctkwjx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ivsydfpi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3euurxwhc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3glusgwcz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3eavpfkdw.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3zoepfnjq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ssmhlzgi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zevtiqrc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ycnjqgdn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3klpkqlty.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rgxpexyo.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3lxsmyink.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3wceobzcr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jpuktgin.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3aqvndxem.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3gsybjtig.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3evpzsbth.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3bycvypfw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3prnnbtbd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eadzyltc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3owhbaymq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3daqyonkr.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cxgrwvkp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3marahiex.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ncqsyxya.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3snpswvet.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3fhntxsna.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3cxmhvgqo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3whvxqxdw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3sogzjgng.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zvfpwgne.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ogwumwbr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jmygzoin.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3iwewouaz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wlytiqud.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lwaonlje.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nezyfega.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3bmdmlbzn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3kcmwhosh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3iosqpduw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3uheoiabl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ukzunbcv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3tcepjmaj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3kgsmwnvo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3bxcgppdx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3nahfeagg.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3jclrjgln.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hidqiytg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3luxmbvyr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fwtyacai.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ujwmnaoi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fhjparls.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3usheapbw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jtsdepnr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ymjwqgyr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ywkbnkhw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rsckptel.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jaqyrnum.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qshbetwa.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3wuikyapl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3sbjwirkl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3msnyhwqb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eyjbaotl.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qtnkycds.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3bxzdgtme.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3tuotfrir.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3zvlwcofo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hhcegkhu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3qublwexe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3hqkpamwm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qcktkuky.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xuaouimw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ngiagxxi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3vsnufkcs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zmlzobci.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lynxhtlp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3izthrgoo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3qwnuzrly.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qwselkke.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3mnubsmqn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qdheofoy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3visxzgao.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3pidctrox.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3mgchuotw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3aoryopcx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3memjhmti.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ssdhiqwr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tfhwyyyr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tpikwfsa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3szutdlml.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zqxrdzoj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3wzxkpadq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3actihtvw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yhlmycsx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3kogcunpy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3tulvtcvs.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tugwdbaq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3vnbmjxsl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3vnpdqcft.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3vmxexdcy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3zpjahfoa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uljosqta.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3hmfvxexc.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3jxswnozp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3samdwpsk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3rutsfazk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ycwvbmxa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3vptqixsk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3pwozcqcw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3enxlywzp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3enhtollp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3glwgdosz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ufywfqma.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3kwoqjlqt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qidgwbut.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3sufrldhl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3zftmblqy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vpszjufe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3stbywqys.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3sorlszki.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3bvocxbam.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ebcwdcgv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xksjvcda.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3pcrflsil.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3rhlutxnp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3llkxrgvl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qtbshedk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3mqrwcfbh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ndshjisd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3vspecbbg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3lkaihgws.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3nwyxjfyn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3zbcfltqy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3efcbeykl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3atrhkoyf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lufwuwuw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uudiatku.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qyxgfzyz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3riehyhcv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pnunnqtb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ddccajlv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hjmphrdg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mkpuykdo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3twxerzjq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3muljfyhy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3astgoghk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3csrhvfpp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3sbndhsfw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3clyhezko.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3wnfgpyrs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3bankgqnx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ubgvswmo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oxsdrpbu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tzshglvb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3pcthqspx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vstqfkjc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3emudxmgy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qyptyqgp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3doodmugf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hdwcdluh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3buwvqnrr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uyuwvcjg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3krhrtalb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3eqcirccv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3phykrina.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3cnujxdbd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3mugbxsbu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3cvsflinr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3emjzvzpx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3svrhopiw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ywfraxkn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3xfipseax.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3edqrzzce.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3kvlibtaz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3amjwueok.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qnuwbmrr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bbuqexxk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ddrcmkjc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3acqckdio.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ikkbfswu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kqnmejsl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3szawkmbg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3alqolprk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3giwisuvi.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qkfuughl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vsalgzhv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3nxiduoor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emaklhbh.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zetcwyfb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3xuyxolnv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ybsdkaws.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3iypyjfbk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ahjmytzl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3gwdihtee.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3bpxrshkp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qgsoxayr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vquzjmnh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3gupkggxd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lllzbbgt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3uqemmesy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fimqfvrh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fijauknz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3foykrcwp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cxfvqmml.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ffolhttp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ppkwckid.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gbrokykv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3anusigsu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mbcpeunn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nkvneufx.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wdflpmhv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jvjniyue.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3lxjsmpew.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3imshrqet.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bxabvxzv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3fxmhuuol.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kfawmxza.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3pjxokahl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3itppxyob.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fvrkxzkm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3autfvpjj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3xrqpwodx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zmntdbaj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pbtcohgz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3gjijpmpt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3gkrfonoy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3yelexriq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sydgpzin.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3kxmjgsds.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lhnfqldk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3uqpudxru.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gethctly.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ramjmdmp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3cnbipfvy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3saxkerez.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tjvrotyi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nityikya.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yqcmcbgh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hytnsfze.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ptnzvsok.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zaxcrmxl.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vrsncaly.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3esxtiqem.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3fpvelpku.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ginfqenh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3hdcexwrg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dtqupfxh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3lbfmweee.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cgevndfi.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3cgkxyrgi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3eeiekxfr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3pdjjfjfw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3zlsnliwc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ytqnhuzg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zizsfuqz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3odvujlgy.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qmtmsycc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3nrjlsplh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ohwlnick.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3scbuoarr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3jdvloosw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jijstyrp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nrohgcgs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ihikxkxn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bjurzdji.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zobsaqsl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3tntkdndz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3kvrljmwd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3matoxkpz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3kljhycsv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3atgleqqd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3hiiweavu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sxytuvdh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zinoysiz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3henvqjtp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3toieqwma.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qcffwsxq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3wvzxztnf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3izrecwnk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3uokwvwul.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jumibmyc.html


<!-- 参考信息 -->