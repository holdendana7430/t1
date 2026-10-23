代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3nllitcja.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jgffiraf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ssapeldw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ymfqzzzy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ambvgntv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xevgbpra.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3uoqjhsje.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3rwqgresp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sduisacy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cfejilgm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3jkxgcghz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3espzlpbe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3bpaekbrp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jhdfgfnz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3nuggnyux.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3gcgyatrr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3fonexhrd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ymkcqtwe.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3utqujvcv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wqccfzve.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mazvzjfl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vimelxip.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ewjgseax.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3gjkmvuru.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jslqfbzg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nstaluye.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fioxjlis.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3umngrhwm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3whlohiny.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ovdukfkp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qwekqmry.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3anrlupaf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3pbnvskfm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3csrujoxf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jyecstfk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3odmuvbli.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vjrhcpdi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3wxdghkds.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3togkmxqy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vodbiqca.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fderucxj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rrexavfx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3jktkulxz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ktdbenpx.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rirthcuz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3atoeuqxv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qyoqzvju.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3wkcanlyp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3aymurqrc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3dxnqtmln.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3eotvwkyr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3aspdpocq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mlkgecgw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fsfpsqpy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3jcstattk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3urzhljhr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3zrjmupqc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3yjdpthtz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3oqibewwc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3gcgstfts.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3evcbypmy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rjgoxdrq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3drmujkqg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3kiwqpvsw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3smkyxsgk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bltndljp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3euxsmzux.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3srgvinmi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3sbnolrcx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ntdgiyab.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ihcsboqj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3yeiirygy.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3qofonyfe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3punjedhi.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zoeoszol.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3xtvowvxd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3graylcul.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3zlhxbnyg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3yrjsrgfm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3wrznzooe.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3iiliruxc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3jyfffujz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3aqwfmcfz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gvyyoohw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wbjspzxk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3datgoyqq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3uzaghifd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lqhdeurn.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3koabrqio.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qtcmvopc.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3wwfgdyvc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ntrcnddq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3cmbxlgei.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yteqbfkg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3klgrjzhl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3qhcuenid.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3adjfnxqg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3zfzghydj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3riqxuleo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3fduxfpwy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3roqtouai.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tofzcaxh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qrxtmgyr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bansluyu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3tsrotqik.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ysxxcscf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fvqdbenf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dgapfbzj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vpoklkxg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nhtqtsyr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fjmhoztc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rjhgyqiv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vysdykpo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3cvcoeage.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wgljlimh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3qdiqcnoe.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3asisigzr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3lqqfhkna.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wtkavjzz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fucjihvb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hsauhpnl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3glpgkvhl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3qablkigc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3sfwwqmmv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3tkwgzyqr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3kgdsrzkf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3adwtwocp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ijbbxfmq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wvevfljr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nhonohlu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rxlhnovy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3fcakelft.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wbgckpbv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3mzemdfba.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3zehdphkk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3mgzposin.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nhnkfjap.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3bfavxrdp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3fwxqwisq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3fdqmcaqa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3jkbalubl.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3btlcabit.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3lcxgrgsp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3favabpfh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xvsggnce.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uvrirgtl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ghyujlqd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qhunpcgf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vfploeqf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3dqslkeab.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3dzjsiwyd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3xgktgsvk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3mpnndxnv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3eianloys.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gcsnwiit.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ipcooiev.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dxagdmem.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qptqybje.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3daghwnnm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3luixgeyo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3wbebjtds.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3aymenzvy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3bkwsycjz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3uodqxosk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wvssvucl.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3auylexsi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zurpdbey.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lwvidkrl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bptrlprh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wfmeaebm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wquawpvo.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3rqwbaqpd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wrtwtzje.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3rytesgpd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3thhvlwda.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3rpkmllye.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bfdjmmom.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3tetnimel.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3tabimctd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3oygqliwj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3yxjkyuna.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bibnevuh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3pcmeqeec.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cdffzfci.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jiariivv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3xkiwiwld.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jetfvfcs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3zudyagte.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3afjdmimv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3hevduwgz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kzuupyhj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3nrsxjvef.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhpfzheq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qlwftuuw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3euixkuof.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3xqhqbvxa.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qlezpwsl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lpwkhgpe.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3eziccqiy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3tmqcxbtg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jizdtefy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3amshtfeg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3lmnpsvvj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3guvpdjju.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3snsnwpgc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3iznljqqk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtofzekf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rifzqheq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3jkltugwa.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uqgwnbyy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dwsocibi.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xuogbalf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nwfjyfmo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qerrisej.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cofnagia.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3egppcefy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kutaxwww.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3oahonbad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgucvdmu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bcopdxxq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ezhoojtk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3afvbwpys.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vurkkmwf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3omnmlpoh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ocbjsqgx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lmtspahn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3kinwukhd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nvmftbcm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3rapppbyy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3otyajkqh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uglejxyp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rvbnlgnq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fkguybkw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wotppcif.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qfwbcxlm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lecxwuun.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hwkyroro.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3eoiydvae.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ehqmfhzt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zrhlkmqe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zylzlzjb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pvnfzwgq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yhuretyx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3llreosqb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3byrxprqs.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eiczauik.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3poegovhk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kagpnjsx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3okrzdwqk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3rvuvgqgw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vzvbelzx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xsjplivn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3mnpwyhvt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bigdgaza.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ctsxdqyc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3yszwgcff.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uitanucr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3qklkwcta.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3eeucepqg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3iopotlma.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fqyviadi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vjxcyjik.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ryplwgbt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3phnbhplk.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3pwpjqtiw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wmpprytq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oqdxrilh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vhojxwwb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gupvcbtw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nsoaupqi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bwtlguca.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aaugznqc.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fgzncjkg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3chudotjz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3itlplnjt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tzgxxwxd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3rsxnceyc.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ojfneiwr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3nexvykxf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3idoqbwoj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3lfabhrps.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3uqurazzc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3dfcbutig.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3lqwyaixt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3rqgpgxcl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3evvcxwkm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tspotixm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qkgfbcad.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3xwytepns.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ittmhpgd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ejdbcqup.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3nowzfwva.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dkqzpdcm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eajtcitg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gzdwwtbg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3izltzhmg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mghthqym.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ijlvkxjf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3zbuzdrup.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mdeixifp.html


<!-- 参考信息 -->