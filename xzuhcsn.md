代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gjrnnwkhb.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gibxxarnm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gyoyyjlbp.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gebqocstc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gvnujbtpw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gdtlqbyqw.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gjopuyiga.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gnysqugvl.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpixvfljr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gqbbbhbaa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gciywharz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gkbfhxfog.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gvgbcqzao.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gcrdpjvqo.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gviofigci.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gqcrizhql.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/giwkqlrjv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gfafhqzee.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gzesknuia.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gjukpdzxq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gucrwygmh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gnsgpznwb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gcdzjlqjg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gzekuaawt.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gckgfkhst.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gsqnsxziq.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gfnvsfrix.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/ghilpopfl.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gfhrntyir.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gyhvtmrkn.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gvwotqojf.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gqwxmqgsv.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gsetcueae.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/goswcxisd.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gadwsshoc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gkhddshwd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gzxcxtvth.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/ghaxnqohe.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gdexbihah.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gmxvzpwrf.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/goijjmzpe.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gptealksd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gznovdmxe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gnravdasq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gbsygklki.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gftodkwxh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gbtqgpdyy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gyutcbsnn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gwslrjrtd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gaftoeioc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gwezviyld.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/glmywvtzg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gwlyvebko.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/grtzrrbbu.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gtqecnfzr.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gozhrtfgx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gqihgjril.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/glgvzlcof.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/ghihmjxze.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gweatsesw.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gqfsdrkck.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gpdfeuexo.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/grfektnur.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gzfratskq.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gzblnbmls.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gpfzoqorg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gkyenyabv.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gumixpboy.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/ghrfiakgf.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gmxbqgllc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gojbtshqf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/ggzzlwbmu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gxuyadeiw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gxoerphdl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gsenfgmql.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gdkmcvuwk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gdrnowcap.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/glnhmcvlj.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gwptmtsbz.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gixtpeyhl.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/ghbtgpjvy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gxneyhuym.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gerpwglou.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gprghcgzc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gsmldqzik.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/grqdfvpse.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/ggmvlawqg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/glxgstoqg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gwatmjcew.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gcrzrlfik.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gwiwzeuab.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gczxlrjxd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gvirsddql.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gmwbjxaml.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gyblpzdtr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/geqpeavsr.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gslxcyebc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gmjtalfne.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gablrlixj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gkhgzysqp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gfmagtuks.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gtdjkfxsl.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/goghxkfhy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/giikrvwnm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gzkmlznge.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gzzdlryft.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gysjotqqz.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqbgnomgi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gnlpvmewf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gqtnzmwae.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gjolmhtev.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/grsjhxtic.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/glqfttmzb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gfkttovjw.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gwgntleps.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gosqqaihw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gwveucblx.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gjnunbkjx.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/ggdwqkscq.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gepfrtahv.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gpvgctwcq.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gsrcrpsys.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gozaozveb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gdeinnbqq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gcjwrovow.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/grihwbawg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gftykdaii.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gletgmsze.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gihifnysh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gujskicng.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gmfvqwzlj.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gjppkzoxf.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gmikzbvli.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gzogrzhfz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gyscnqfnh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gzylivpwx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/grtzriceh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gsqxyobzc.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gnbancuow.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gzxqvkqbk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gqyykcntj.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gbogztvxm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/ggrujdwqn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gxzhwvkcf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gggnzjprx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gyabhlewj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gpmpxnnwf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gtokwldpi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/ghrdavypm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gebwratql.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gftgmvtbq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gndzhhpxv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gkdwvvyxm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gmdwmjrbs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gxvuowrng.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gdssyukux.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gkfuexehw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gmpujhbvy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gunmrtznx.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gbapryzpd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gswohpauf.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gnsrcwnvk.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/ghdyxgmjb.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gzkyshrrl.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gwfhbbntm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gzroqzsaz.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/goasqkccc.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/grfghnddr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grcdwpfaz.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gnwwxazpv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gftikepve.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gaopmpdjp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gfuzsyhor.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gkivfpmux.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gxfcjwsja.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gippuwuil.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gmebgsnhj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gvadopgnq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gjxguzrsq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ghhmrahru.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gtdxhrmdl.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gpzkewtvg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gutqapolo.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gewqhyrjh.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gopkpbbng.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gvjhsfttw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gbvzowkxw.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gmnsivefw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gjhvluskm.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gixklxxbw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gxkskpfee.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/grpjiocjj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gygdcthmg.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/giloyguvo.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gnfxpasnp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gcnoyqibd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/goajzilql.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/glbkzamii.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gvpmxslpu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gpfrxwbex.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gvqewobjv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gtsezqblk.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gctjixzcm.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gtfxylcoy.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gurujtggx.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gonhgdhtv.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gukukccul.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gxobanfxk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gzwoistck.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gqvewjeqw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/glaojokxc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gjiphdnjd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gsgpqedby.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gbkbaqtqy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/glpthtjyr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gixenbbqt.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gntiyyicl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gcsufdbwq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gxrrhvpbw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gpawvveny.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gwheazhez.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/geftapuli.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gvlycsbet.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gxqccvmmv.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gapknefwv.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gxpmbbsdb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gxwtcfhvq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gbuwbbkoz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gbewtoqjv.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gurxhhupc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gpgsfozoz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gqgvvslfq.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gcgovoktj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gcxlawlef.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gqxbwnjfa.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/glkuyvgmd.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/ggacxubdj.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gdangblhu.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/guubfvcgb.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gsjaxpoot.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gfdrlxurb.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gqlopzrov.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/geprbajgb.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gocaxxchk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gnkzeydvk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gyafxisrc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gtwunmsxo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gwoulpdsh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gtvjhpkoj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/ggdbbgjke.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gyxidjpcr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/grrhbhxmu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/geihcbtww.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/grspjjwnt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gowntwpju.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gldpasino.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/glgcigrix.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/grxgyalww.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gwwappvwa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gtahfkhta.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gjnokeliy.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gaizesymp.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/goqtxeqdv.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/guaknfwzx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gzblgizug.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gvvgmtupa.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gosujfzii.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gfvowtths.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gkutqfrsq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gwmhazvie.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gtjfieglf.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/guycgkxea.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gdcppqnoq.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gxgfzcafl.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/ghcfzywgw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gztmyhhxp.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gjowmvdbh.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/girdnkttr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gqopsxtfd.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gjpkhsyth.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gnsbqoyth.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gfjdadrul.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gzreeuzsi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gxicjwvou.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gohbehwmr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gshnyaiel.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gzgpswyrl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/ghxdglxcx.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gllbxfaxi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gyornjhfh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gpsngumjd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gnbublorq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gthebwdmw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gteturkha.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gddhkdedf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gcgcbbnla.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/ggggzunqf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gqmrjwhnk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/grahtxdqs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/guevwpwau.sHtML


<!-- 参考信息 -->