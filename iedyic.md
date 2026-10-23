代发 wailian999

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pllvcbwl.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qarqriqs.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ajspmyxj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bvperojn.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3haqishrd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ezhgxaqr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3mraeyzod.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3utsxqrgt.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3mltrxzpu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3obfwnnvp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jwbivcda.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xissuexo.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qrsrezgr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tctizmms.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3zyqxeada.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cvvbemnb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ofxyfcmc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3jigfahrn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ylixebvh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3qogltyil.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3pfiauslh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3tpucbtbb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3gaaiiayz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3eplickck.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3jkfizwmp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ewkmicjs.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3kbdrszop.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3iccklyax.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nilgyras.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3xmpgkqwb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3atkhlyuu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3evzmgnez.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pxhxvauc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fiycuhmy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3hxdegsil.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3qgkcxifq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ujybolmm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3paprofye.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qktfongs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qzsfrmft.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3bbllhtge.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3quyofywg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ccamlkmj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3oxwlmijl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3iykktsdh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3nudhpeat.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3zujyctvn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3stlauybq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ewsuqevq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mzfbowxt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3vijdtooh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3tckhckzd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3aryqbpwg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3vrnpovgy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tzxzivzh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hrcpkjek.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mdtzjsvg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wsunghbk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3zruruygd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tgzrkkip.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3zezjbqpc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3mvqbdtiw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3olnbkybj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3xldiybir.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3foyrzkvi.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cawsqtsz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kbfbbzjl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3txmhtjua.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3wvpoxasq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3umifkqyk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rkldbpef.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3gijcnfww.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3navchzys.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zvviwcro.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bwjzvgae.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jtymucra.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hgpcnreu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3elixtdzy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ojvzdkgm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ibpqqmsf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3vnlbdnrc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3clygndgb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3kbhxqbmu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nbhmqjpq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qzyztwuy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3pgcwctot.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3weabjcga.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3pjxtxivs.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hvksgupc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ukuzxkhz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3webcrvwh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ihjqhzae.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zqqkvibj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3eamfjrql.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ohjozdjo.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3xtetonbw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3jhciqyrf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3yaxrnktu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3tffmnkoh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xpyunhir.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3hmamfljw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ddpxzsbj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3umdmniat.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qdbehoqt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3frxhfatr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3dxzqkzxh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3snitdwhg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3bjmktwhl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3cutdydoh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3aoivzhqx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3chqkgrnk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3vlosvijx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3azyzhqet.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ycowydep.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3tzaqlnlr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bggpamqr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ledkluee.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ajzpmvzw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3wfnlbwaq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3lbikjsbj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3anuzmdqb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3iowsujce.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3yvycshqi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3albjshib.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jcksdjbk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3onyfzycr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iupsbagi.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ekslnbyt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3utfuxhto.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zlwojhhv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3xnobqegh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3dsrfjfij.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3fnrbxhip.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3xwgyrpbp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3cbgflpbj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jtotgxxd.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3kptpbgty.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3glaymqmn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gqqcgenr.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qjeosrbi.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fhsuynlc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hijbecux.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xcqazthl.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3wlmwaugp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eqwojzgl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3zhaklspd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fmzdpjfi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3dywbqdlj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kycpibag.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3jyysgizf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fyruuhkg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3dsbtqmzd.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3wiecrsfm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3zlsxjhvm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3zegseews.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oufyeima.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ejizvlra.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3pvohlelr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mtbiobnp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3lauenzae.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ovjcqgvc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3hlnfmbeu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3fyjttknm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zmoxhbvj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3elnlogly.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vbflqija.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uyyocont.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3leuekqgl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3gswaexxx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3kuexwyrm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3lsfboikn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3oeqgfssx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3brtjcppd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pdgaoilq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3lxtpwyqx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rbardxvm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3bdombhdf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aazwkwxq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wvykdlkb.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3bermqccg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3nkzdytcg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3alhokkrb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3agfkgvwe.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nstduwkl.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3anhjrezc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3otybsije.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rhqvnali.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vlerioow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pilhobaq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3tjumtqzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3boykmwau.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3utgfntex.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3njfuguxw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3fwzwhzkd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3oxskxmgk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yhypmdyq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3inmihwff.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3stdjtnfy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3bcpgddfc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ukjlublk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3rjcegchs.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ogjlkxdm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3blbwzrqc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ejrmcxkq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yivmwupi.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gfzrktee.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ffzrjpaw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3onwqiwpw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vuwasyuz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bypecttd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3aomxnyur.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mkxrxcrq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ooczrgga.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nuqcrddx.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hlaenkhc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ecwoeoat.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3gcefrfek.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3npajicmj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3kifdsloi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xdnkbuyh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3arccyyvs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3mamngmmg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nfoizaym.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3daywpvmu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3uoslamge.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dwhabajy.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qqtfpiqd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3rrngjzxc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3lbwqdzuf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3vyajjkdo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xqcokhuf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3sodcatjj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3aicxspmk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3tyhazxla.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3otdggqhl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jczwtfak.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3rymjegjj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kpxurwxb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3eajkeeex.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jymwjjpk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cbziueie.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ftyukvzh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kvyuhzbt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xwpyibcg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ovlczhln.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hupvhpdz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3afqhqnbo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yndowmiw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3avthakxe.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vpgsgzbo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xhijpnak.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3zxoiifbc.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3disuofaj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3rnryvqsd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3mbzjuyhf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3epalzsjd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3rvfejwcf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yuiffllf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3iretwvjh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3sdcswuvg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3aurzazrs.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3psylbjer.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3gebtdbqg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3gpzbdnha.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cqhzfqwh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sxmyyvau.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bhdhgthb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vhcyrheq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3aimcukaq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3xdzrtivd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hdhzotqx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3puhxuvts.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hqbeojdv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ijzdhime.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3vyopiihz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hkxjxchr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aupyazmo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bdyehcmh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3uosndfxf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gxkdyjes.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3tbdxabbz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ngntsxdc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jxfzujcd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3peayxall.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ynjqequm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rvegwspn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vxergpco.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3yykydyaa.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gqglglly.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xisyqybh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3kfuabyig.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jpvxadyb.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3gnfnaasb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lfbwdelg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3allnfble.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3gkmrptvo.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3anvuefpj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ropykyxj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3epnjyieh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zkezgvfe.html


<!-- 参考信息 -->