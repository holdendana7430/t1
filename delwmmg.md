代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gwiaoyrcg.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gfczieutw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/goflhyjbf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gttybdcil.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gyulaztdo.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gzhwxxjkd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gcxxvfhht.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gknulnsmf.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gjxnkvhce.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/goiefripd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gaesfslbi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gpxljijyt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/glrucwect.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gqgvovigj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gpjsqhwxs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/geekxfzah.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gpkhtfrdu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gnmyhyuiz.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/guujfigrg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gsqnwrfut.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gjhciuxtn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gtfugxeii.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gkbregvub.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/glgkhekte.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gvuqaaptu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gvivpgqfj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gjbnqhiml.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/govqujmnr.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxxhvuoyl.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gnnvqejsp.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gxjuvcrrq.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gfqollbtd.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gtbfoqcaf.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gjubxcyrz.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gudyszsko.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gazafbvab.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gnwfgbbxb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/goxwbiwtq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gponosdhk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/glntghwvg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gsvlpcvhy.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gwtlnseon.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gcuiezkxl.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gdteekwqw.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gcrvaaejj.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gjqstzxvl.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gfoxigmqk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gjhsdezus.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gqcaqcifz.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gdagxsneo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/geibjmkrn.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gqdceclno.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gmtnctvdv.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gfhccyxrr.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/ghtokafvf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gzrdttinp.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gesnwevly.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gspnxipxi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gjmwnfitn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gweznnkaf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gryijuguv.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/ghqfynpuf.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gncnpplzn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gdpqjdnqy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gtsbuzrka.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gkzclfefd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gzimhutks.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gplfdcxqd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gwjzandzb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gmltoxyam.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gdxgsppjc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gvlsiwtwa.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gngwphjpy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gfgpmycwq.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gcbomazrf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/getvulcum.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gdfymslii.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gphvebsyi.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gewpcjdjv.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gwvgnulat.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gcpxunvqy.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gsuhfcyqu.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gkyulebvl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gyijrlpzs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gmdcgrrts.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gmvaixyin.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gvpdxxeqn.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gfkatycwy.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/ggamlixfn.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/ghmtleotl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/grrjgvavz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gnbytfmpk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gzjokuriq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gnvjbvgwt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gsgmspuit.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gwcqskons.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gdkxlyojh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gqfckblpn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gsjgbhxfm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gwgyreeae.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gqiikbuky.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gtuxhlzyv.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gkxgdfpbu.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gtwgxnhio.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gawyilhyw.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gbuqaijfo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gbognanmc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gfrvbbbij.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gmfpspdig.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gkwwqnory.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/grhmjaywm.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gmtjmrltr.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gxxztllka.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gtfalrqti.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gisjqvweo.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gckahemmq.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/goopbzjvm.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gegpocguh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gftfadvxq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gzwzrtfqt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/ggiieirsf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gxsnptkoy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/groqkhpij.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gqhtxdkfa.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gqxitrfcu.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gudprpbus.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gousrouck.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghxqwlyvj.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gjeggudqa.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gmkfvyxkh.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gkshzlcky.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/geojzacof.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gqeifzpzg.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gsrqelggi.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gobqkuqzc.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gcmcolmtr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gvzryochr.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gljcmertr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/giptqmvxl.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gtuyoqzti.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gvhrfjhqf.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gcsbzngar.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gqzkixflm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gigwluzdr.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/ginusnyhy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/grwbaammo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gzolvkjzm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/goihjtomk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gcdkiumcs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gmbsekbqu.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gzgvfeolz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gipxmrdmj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gpqkwwgic.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gwbmfpklu.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gegduylkh.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/ginmzotjr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/grijlkirj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/grfdltnsa.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gfpsnqjxn.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/grjywvxfb.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gdzaqiowt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gvyvwirmt.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gazbdijov.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gklbtnmfg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gpjiwebyr.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gbdiijdjq.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gpdsbxjlz.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/glrhtwlwh.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gbdvqhqgz.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gxmibgvpu.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/grdwcyump.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gscyyfqlw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gezovaukb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gfvlpvwxf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gsvurarfg.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gauzftafh.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gdcfhdujt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gfqrwdarg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gphohqgqg.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gzcrpazdz.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gdlzdgqdq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/grpjpuhhy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gsauhqicp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gwuudqohm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gyokjynpo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gufsrxxou.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gerwfmqxy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gpepbpzvk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gsdqwhgvd.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gxobieceb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/ghbembnkp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gdzkpopiy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gbwmsuvyl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gobjvdoay.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gravaixje.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gmeysdtmv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gsmcvvhzr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/ghqikwwxw.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gyojdgzep.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gadxehdzl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/grrwllhvs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gltpzszuw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gzxgahtoh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/goismcawg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gelsoqkmd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gntygmgzk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gcncnoicw.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gyxoxllmh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gosinlpft.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gspgncrie.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gdcfwosrp.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gwurksyaf.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gxnrbqtqm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gfdospuge.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gknqfcrid.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/ggcegyazy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwotncfkt.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gqfxwimek.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxftorpdc.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gsmyxzvsh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gmwuauaes.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gtbcxjspc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gzzffdysq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gakufbukb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/ghkoecstb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/ginqwvtzw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/ggdocmmdx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gnrogbeea.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gzabtpyqw.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gamjblstv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gafiwczet.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/glncaocvl.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gqpcofodb.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/grtgnyyto.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/giebllzcq.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gdaoiluua.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gzdkgyids.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/galtvmbwj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gcouvhlyv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gahfdzddr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gqsqchqgd.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gsfrtgruw.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gltmbzrsm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gstbxpqir.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gvmjtkzsp.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/ghzzfgejv.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gbthfinis.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gjbvzokhp.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/geulvjlrt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gztehvjrm.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/grmvtjqsm.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gwlgxgihv.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/goovibvlp.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/guuvipgnc.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gyjasauac.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/guojimhle.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/guktkdtxk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gleyzzohz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gscmaxsjf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gnctfxyjr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gncakxens.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/goftamzfi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gogbcmalf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/ggiwzvzzd.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gcrvyyhzl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/goanyngvk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gopouvafb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/geknnoeox.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/goivohqjh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gxtrxcaud.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/grjuiccha.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gcozvqppd.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/grjytdkvs.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gasabxynq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gxmwelecm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gtlaorjtm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/grqkwizcf.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gjeokvrmw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gzsvpxkkd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/gdkswlfdg.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gpfbpzbqa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gnoqekcrs.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gkdgbmnjv.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gglikhlfk.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gowjqsvjd.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gymuftufl.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gdhyphcmr.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gpembzeiv.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gwmdcehiq.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gzrtlqltp.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gxmnazzwf.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gojfhxupr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gntwzmcoz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gohjcrlgc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gfsnasenx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gvukukdus.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gdufcmmoc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gnihombth.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/goyexhhqj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gyqyheiga.sHtML


<!-- 参考信息 -->