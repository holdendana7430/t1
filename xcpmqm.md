代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3opktstoa.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zthntutm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qijbzioh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3iabsrimy.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ejjriyzv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ntpjjcwt.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3volswzdx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3gdyudrtw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3drueenzj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3bjainjxc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3khndcagk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3lasxrqxx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3pnwjifvj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pywepsqv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3btrfyikt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fpftiado.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3hmjnzqga.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3cmonpsoe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3vhgrhgev.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3lznwnzwj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uofkstrl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qubnizfz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3lrmnajyw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3rsnhhwtj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rndbmmnj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hmjoendo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rsgnrlfv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mbfsiurn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3dcnzrnyw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3roemaztu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3flaywvqk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fyctjovb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3lkhyyzmx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3orsezwla.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nnpmsrxn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3tvmqihev.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vzrnikkc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3qmowyiyx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3qgnxcyvt.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3whsfbbbl.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3nlixivby.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3bptjquhr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3bdkuysxs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lcbzqxbs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xxmihwjx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3iijjrssa.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3tjaajlpl.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3evgkoryv.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uekzqrcc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3czvcguby.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3flojcuip.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eeqtgecl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3wlwuljua.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3esaaxsgd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hxckblup.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3mvtwwblj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3wngniild.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3dzmxuszp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3knmlzpfl.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3tqekweod.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3geuqsxgt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3iphyrycq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3iywxaokq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gqzobiut.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dnkfxgbp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3zxbustvd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cjoaizts.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3luapdfze.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3muswhega.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ejvkyiji.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3qahnzkfc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hsflcaya.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qiwwrlsl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3eearxfiv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3yzfqbbgh.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3umhcgvfb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vmnyinyp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3sqfkbndz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mmclrqfn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ldzhxnqc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yiflkoax.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3svigruqj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vyotctia.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ebnlcxpd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3zkisyhlr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3saasyehx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fgaegorq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bpuynmmt.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3dsmwapit.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lfdxnyav.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3xqjrjwoh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3psuvyjyo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ekyfntms.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ykgrheqx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3mrbeeqjv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3iobecnpa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3dckbpgpb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3vqfmnnrv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3qyezpsgu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3nrfvnvoy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3xdlpyoxo.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lwcmuepn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ubeapvkl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uwhdupjj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3wuhpgbjz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kxlpxwhv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3cufwlkfg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3lihldqks.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3touhbazv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3kwqxixlq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3rwmacidc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3cehwstjk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3cfjizonh.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3cczdnzkr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3aqcvnabb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3rlwiymzg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cvnuvdzj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mogdgmso.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3tpxffamf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3axqdbvva.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3tesluhqr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3duenyqsf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3yhgksyvq.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3perrtunx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3rtyhejgc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fgbddina.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ujogoozo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zsjetede.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lxynrskm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xahwaeth.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rwyotjeo.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3icwykwas.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lfqqiljq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xlkhjmnf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3mfsnzilk.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3htvdkubi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3diubmylz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3whvtgeuz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3lokqgjsp.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fmpecdsj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3njcuteec.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3gcoueiuu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3agkqivkc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rsomqynv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ibtejqtv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3itxshifv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vdvfrdsk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3wvgjgcex.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3qespaexe.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3qbqyngjl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3pfdztxio.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ogzqcdha.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ygnjlfts.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vnynihqf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3kxpijffa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3jhdvehoe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3escvgclo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3xxiyzari.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3hbsxkdeg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3mtljnaaw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3glqaoyze.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3hixmcqlh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3nezigluo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jswpjfll.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3xuflbpdd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wvphpzrq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hmeedflk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3piuohwcv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jmdidaul.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wbcpntes.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mmjzaluu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hxbgxprg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qlhndcfh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gcrfcymo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zcoqlyor.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gtknaqiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rkunprxz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3mkzcfiuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ilfmvvkr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tfpgvxun.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3rrpliowl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3rvfuvwha.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3eotkrwek.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sebasoqr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3llfjinob.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3jmjledqc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3wjoiadmm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cbukotzb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ybqtdapr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3leigcbjh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3mvkwgmgq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qybzjhum.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mgtzrkzn.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qqwoeoav.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3wvbyexsj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3iddajlwn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3iqgxhkms.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3yxeijlqw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rxstdksg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qtptysly.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kkhjdvhh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qhkwpizi.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vukgxxvo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nqniwexe.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3mgslpvaw.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zmazbkby.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3zpveytfw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3briitsqk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ztlqixlm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3yovbqhdj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mnomxwqs.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3madrodbt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kohsmphs.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wewixxcc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zxxwoazw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3vvauxbjw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3skkrwzxx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3yzesddbw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tvxmdfum.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3lgnrtxfa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kczfjqmq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3leutagdd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mimqgvja.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mfnuswgv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3zqietyqt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3swgitakc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dadznqht.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3djpietxd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3swvkunyi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pyeqvbrl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qcdjxdoy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tmhqixxb.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tbizlgzw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3trprcnsp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3eailtyae.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pxseglau.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3rdcqpbxo.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eyanqkee.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3mduskwhp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nyryhoug.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3tdaardxk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3olozutwk.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3emunizsq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3rnpprlgl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3grdnfmnt.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hckncory.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3izclzjzb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jvrpvzuj.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3oxcbfckh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wcpuhdnm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xaaroxly.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3tjjrrupg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dzsbsfvg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3qbeuajoy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mqtlejks.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wvtjqjkg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xkzzwhjq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3mwkirmas.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3kntnppbr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3itdlwgxe.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3jzpxvmnw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dmymoeey.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3tldqzetn.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pgqgzfuv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ervhdgyq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3skenrmyx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qtqtffbj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3akxdibwq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ryqjnxak.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3wytkeuxf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3awiwargj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3gzfbtgco.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3onehzpit.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mzdjhhts.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3vsbjailb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zxziwxkh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rhlerwau.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3gaaedacz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3opyulzaq.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3idthiuwt.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3zqhccrsc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3eybczdol.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xxmvaavo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jlbaxtbj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3xzbqnjaw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zktgewqo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3rsdtojaa.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3gsmfavii.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3njbdwikd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3errwlavh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3symzcmgd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqtpqaxa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nxzmleqn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3vvzpdngs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3yukucevg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3syysatyc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3uyosebiu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3iigcxswd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3asjcjbvb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3eqsbfbli.html


<!-- 参考信息 -->