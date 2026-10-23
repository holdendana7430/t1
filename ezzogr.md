代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ejdjcgpt.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3zcsfltoc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3hnacyzyl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sirierlj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3wcyctikm.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zwvtwglz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3pzbvhfab.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ymkaefnm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3croynnpv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3dqmcsyyg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3awpckahg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vdfxczaj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bwumrxht.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3copazcqt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3fjirfodj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3qpfikplq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3efwiktts.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vwwddtnb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hwgmmdur.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3kdawdpir.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jdcrsqdi.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jptqjwyp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nbhfscfw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3enyyxvuh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3xbzbaevd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wypllkwe.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3gppjxwmp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3malvidka.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tgtdkfqj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3fttxzpad.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pmhvridc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3igftoojm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jxtnxxbh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3krbwzujj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3vewulzda.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hsuyttdo.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3shuwrkem.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zbfsehax.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3cigfbucy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3nzipvjzi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ossbfrzx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3rjlwrvmz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vspyspds.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ylsnwepa.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xwjsfyaj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lonccerr.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3dgqvttgr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ljbjxcer.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3luuygeik.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3xtzbspda.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3oxnfxjuh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3mgqawwej.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3yhqtxrdw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qznlzzgv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3waclmohy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3eoehpuea.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3psuoxbti.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hbqtqjkj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3dopfcblf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ciuavfom.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3rkyoegpm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3fjtpwmhp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3evtxjphl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3dmbtmdnn.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3pydrumya.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3dmylhrqt.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3uvnzxbkr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3hrwlrmhj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yprazndy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oyxhtzro.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aiiehodv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3gmcskxkf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3lezjjpgj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3xaetmfhh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3nnuhbzwm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tjouumsi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3phlozaye.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3tspmjxfk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3uzyetogl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pxhjkeli.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aufnychz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3pbsjrngl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3sthfqmsy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vpqmcwxh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3apmlnjzy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ijnicbzh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3cyzcwbpl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3xkyyxcfv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3nojvfmdj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3jizgmunh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fnqktexr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3jmvbtkfu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3gyrmxgsa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jsqzrayu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tuakhvzt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fjraxzjs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pdrsrtxw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3uufxncue.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ffwfzjzi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cfwvbwaf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3xejlrpze.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fwcxkrvd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vuwmcvof.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xlrihvwd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wejrbnxv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3eknucwat.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3udpmqjzf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3twpwugjn.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kgqhpyrt.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3wzlfccaj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3djcoaxiw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oceyugej.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3arcuakxu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yatceooh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3sddbdhel.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3gbeltvtm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jelbtsik.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3blmfrdsz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ynmctvjb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3azuvpvdb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eddnwlrf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rivoevyb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3cjxvbrlh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3mdpnclxh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3khvluopv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3arnhgwtp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3fnundbjk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3dcjwrbof.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nltjlbye.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3zdtcjvil.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3sxlfytjb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3egyakznw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3jhcmoneq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qhmmxfnf.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ngvepogo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nescindn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3lhtmpmlw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nusjwnfj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3hrbhbygb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3aggzxsjl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tfhzwccp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3uugywrup.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3flvmhfha.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3spgyexfn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3lungspun.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3btzvpwez.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ocvynjfe.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3uqtrcdeu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3disypvew.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3odbxxbds.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3opwfvkmk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3msqbbkry.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3mzthcdou.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3gcfoserd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ciicflrp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3guiazrgc.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zmjxoqxj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gltlhbob.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kodxenox.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hvxapxwq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cenwbikc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3cordedsy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wjldrfpj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3trqlsovx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wnkztrcl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3rqlsxwnj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3avdkzaai.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3etfimthi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3snbpnjpb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3lguvckbr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3xdvuihpx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3inprbjfo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3lvptuexy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3znqyjwzp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3hlulusqs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ytslmxni.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wivcvroa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3wdtesliu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qukfkhdy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3jrdojbno.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3tatsyhin.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3hruzqqjv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3gyrjqdio.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zlwtfrhs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3dfmwikdd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qesackel.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jdpdquop.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ycgxksvu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3lmtztgig.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3bpkhramk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3tynlbceu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3sfnuixuq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jatdfgan.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wkcyktau.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3gkwqnzwn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oxwqaroz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vxgswrtm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wulrovqm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bexbdueo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3aqsfqecd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yojflbmq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ufsaqmgt.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3svdlpvlf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ttoalelo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nabfzivh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3krkkocge.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cerikbqn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3uxvufmak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swlaqnxj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jcxfkccr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcqfbkmc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fidqyjke.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3gppatgzg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zowirgsu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xoieajol.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3gulmfbck.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ijthkuvl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3drzvwekq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3pbfvnrwf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tgmwomvv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jvvtkhiw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kmyskgzi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oytquouv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tumrrbaq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uouiyibh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fmlfeein.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3clpwkzwx.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pbzstesc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3wuqqniuw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dazejpwv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3eayynqfn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zwowifsd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ohkryxei.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3omqsrbll.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3aptxvzfe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ekfuqrvs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3llyrjgys.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qinbwudq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3hcxdkplm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ghnqzgim.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3yqodmkht.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3kawnnydp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jcenzhna.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wsmcgsue.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kqwrcxap.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ubffiuyg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3farfeoys.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3vxzqivvd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3jejbvftp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3cspiuxwf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3topqcfky.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gohrcagq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yremyuaz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3cdsofojw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3pdcmyfbb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tshdxdus.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3xqzkqqbs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ftasnwkc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xgvepdjn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ovvawewv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qakkwxal.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nawwyrzb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwprefyx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sfmllrnx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nvcsaajh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kvccidne.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3evbmheha.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3btwdjxaz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gjfnziko.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3cojyxxxp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3voadfvmn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3exfznrxk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3qudsflas.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3hcmzzuod.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3iwdjkgxu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ccymluhw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3kfbdygiy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tgmgqljz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rgyqrobl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ffxwftkb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3fqdqmxdj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nauahsui.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3agrlrdta.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ikvjxpyd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wjayoqan.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oiwaiezt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pthxytbl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ekheinzu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3riiamwlh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3dgtjznrx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3bqolpfua.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rurqbitx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3nlymhquo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zugxvlly.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3zaddxdmt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mydifszl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dthhcfmn.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kxwnmwbz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qgaqntig.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dxuedxqr.html


<!-- 参考信息 -->