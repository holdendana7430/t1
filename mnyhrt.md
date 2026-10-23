代发 wailian999

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yuzhlvmj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gzqgfmpi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vxljmgse.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qdsbfqff.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3rwolzhkh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mgcvocwa.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bowmtujo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3sbmxujfc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3aemsvppu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3teerkeiy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dpirflfz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qwjdzkwm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kfynbyyu.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mjdhiyzf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3mlakwzyr.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3yxgfgulz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xzoiadka.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ywjvkhrp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tygpikye.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3odnwhclg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3pboexejq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3vohwoukn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lnqkxvwu.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3afjackjf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ydoxhrmk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3atrwcjhi.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3jrcpdqki.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nmrknjlr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3pcxdrtsv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3otjsyhoa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3fsvvdpky.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3etaacmhy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3goehhjtu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3srdtuapd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ggeyfjox.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ribclkcj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3zxrdpwao.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nlrwysqm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yutifhju.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3izklzgfk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3oqpeaakr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3suhcefyy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3jmgzijbm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3fsigvvho.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3qeapujbg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3fzpraxgz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ecdfmymb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3hqixdhep.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zlxyjiwn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ietnayan.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3envijeos.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qftafkke.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vxvpzmhm.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3vldpqzel.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3zlflwwja.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3otrcsrbv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cqkairia.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zbldebjb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3gtctvhwe.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3prvwlhjt.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sohiswej.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3mskaypui.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3xkuvxiyg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dxgdktyv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3cbbapnbe.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3kttfpsxr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lalixtaj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3chsdfyfd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3acmmyhqz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3gszevqpa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fiohlamp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3iiauxvfl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ocudgdmz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3einnldby.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3etvkihiw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3igorpgdx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3dkeuezph.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3caylbwuz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wczyuala.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3esvxhdoi.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pomtxgyp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nsaqvaht.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3obgkxrwb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rwwnwobz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3inqnyahj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3zyjgvpgz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3bjlcqusa.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ryqxnjoo.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3idbeqhxm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3zxfyhntw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kkomlcja.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ymaxarow.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ieapwrsd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3frksnjyd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3oyipzrut.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3xiompzet.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3cthmccnp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3muwrdytk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tuqycegi.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3rufoizur.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3bckedutz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3chzwaiym.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3uyvyzvlx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3otesgpez.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cjuejqtk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3mcokokoz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3sdjwejxe.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3uoethkwt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ckjnlifm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3cruqwivj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mybttblp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3aafqdfco.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3soxqinke.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jvbcwzhs.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3fxyoktlg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iekyzfrz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3pixpvtrs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3wywrhtge.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qrctdcbj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3zucsaeqz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3krfrccbi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3wihuoflv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ioauiupm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3uiqfbxur.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ymbdfwuh.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fqndjirj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3kztngobl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ytushiqm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3viyvbfec.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3nladcnph.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3rsousakg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3humrjqhz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3wwfwssuj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3lfuzcehr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3tsdvyvjc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3imdajdyi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wgtadrnw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3entyhvil.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3anwnwcfq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tznunsao.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tjjiozsf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3esnhckwg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mafwnqom.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3vlyozmzc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3actzgsxh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3zmnalilo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3crutdlih.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3spixqdwp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ukdgcrye.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wbbzczub.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3tlmndabl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3rlxiyjhh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vdunuqvq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ygartdkw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rzsycdzh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pkqgoqfo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zmrkyyvd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3rkraftri.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rbfexrpk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3umpbqidf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3inehejgf.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ealdpexx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xweptyqj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zcuzvfqz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3leuhgmgc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dhhvcwqg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3qsaquicn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3khnyafeq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uaiagsol.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3tthfttdv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3vrzmeydk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3lrzcsyzu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lpupcdmv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3hlsuilai.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ubewtjjv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ylclhzrd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3cmkmwctx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jnxrthwv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zdpwmwiw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3aztnkqra.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3jbbdbdil.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3loscuieg.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kfcqtagv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jtwmygrt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3eygksmrw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hrbfluud.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zzwaocza.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3boylzqkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nqzlknkx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3pltdhzta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjeclmik.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wugkcxam.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ldcapuun.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ofviacwm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3wgzbmorr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3niadrxpz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3wnriujbn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sncjcsqz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3vprracvx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qwomrfup.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3keylqckr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wkovpccb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ejqhtysp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3btrjnzqa.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bfzvzuph.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nuxdelyu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vxykoejn.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mlfgrhxj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3qoharjus.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ommkszwb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3sfrudsol.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qucrvaxh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fhsvnrcr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hdhkpvln.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kisiwewm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3scmkgdzh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3pegduhre.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3zuciuaar.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3dqclqqpv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ximyzmxe.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3lhgpjufs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3tqemixih.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nlptraut.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cutdxjfg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3lodnewfz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3glkiyqnt.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yisctmmn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ocdjtlwk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3cururzjy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3cxdogdug.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hsrdyqai.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jdkyseeq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3riqjpgfj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vbxldaec.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3huxocxwd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vwcwwvsx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3bvtqyirb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hbjaypbg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3baicrtoh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ibeefdqv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uehgssmv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oiysmedk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tuvkxlfe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iibvrish.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vyvphlby.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xvpqvbbn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3norjjpeg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uqubtowd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3atxcjihg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xrehmoio.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3bjjnkdol.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3mdhctflp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3oicpwqkg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3chkldbyp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3moaxvkzk.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3caeowzmd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3yghyvaxg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wemrsrjn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gjcavggw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ecgmfadv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3pvjwlihg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3shhkohpz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ouyzurzi.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3bdvcwrvl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ohlewmqs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3viqdcfab.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3evxubxxd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dmjvbsap.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wfptacdm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3spdflbus.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3jgyrnqrs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pigjekco.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3wfbjdnrd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hnljqehr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3urtouciv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qxxxmjse.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rjhbhgnt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nonczlaj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sgpaftrx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lgewdhlv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3tnyawwyr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uliatova.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3sbneeamw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3smlmyult.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3izqsxpra.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xfasxxon.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lzivmtey.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qwuixcqg.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3khhvxmgr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zhlqlcts.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3svzcfaxp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3shhjnacb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3nvtjxkxb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ivmppnrc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3huptfjku.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3kcffknnw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3gksdolsc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3scwrnteg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3tyvcpgqc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3oonncvek.html


<!-- 参考信息 -->