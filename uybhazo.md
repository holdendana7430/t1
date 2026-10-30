代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gavkdzjlu.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gyiquckqx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gonguuzxo.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/goslhbput.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gcwiyqvsz.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gjihpozpl.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gsnhtbtrz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gflzllysz.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/grngnpola.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gminpwmpt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gmercdnga.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gerksdxgi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnegqltzh.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gdyntjhmf.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gapusqeql.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gheiqrcxt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gfmgfmozj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gznwpcsfn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gatnhetja.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/glglmzxle.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gohwivnve.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gemshwxqr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gahjnicvn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gdtxmbsfz.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gcwgyaluf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gxhiungvc.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gtreepffi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/gwpkafitq.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gkondbysx.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gphizkjiu.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/goilnmjjf.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gvfnyzunp.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gfapgwsox.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gkhgiohlr.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/ghoysjtzk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghegfjbft.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gmztqcoku.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gtusiuyum.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gairqpqob.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ggcuqfyfk.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gsmuhndlr.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gxpjbxivp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/glqnluezy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gmgecbpey.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gyswylnsd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/grdlgrttk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gweiqsukl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/glsxcpjxj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gdjjihkbx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gmlfqofjx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gfztludoa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gfwgosjbf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gkzitwdxq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gqxbgecoe.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gewpfbrje.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gektsfyzk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gpithbohl.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gizgftipf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/ggwgzfnzz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/garkippji.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/ghpqtgewz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gjzttnpos.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gqhnejvjc.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gbrrafafz.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gzkodjmoe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gobflfrsp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gjyvwngry.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gobqbqgfv.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gxuyrsqbw.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gbmhalqko.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gjmgishzp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gpsjteyho.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gfhipcgeo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gyqpuayis.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gxufdgnju.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gpvwfrjjc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gnoigffcl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gculjnjma.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/goqgqyafk.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtwknxvtt.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghannbfei.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gjqhretws.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/grqjrkzag.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gfszvsrkl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gzpjvnovd.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gocgefuot.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gcojpgboy.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gacldtldl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gxctdcyht.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gjzuyijhb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gddaczgeu.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gqwsoqkhe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/giimnknyq.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gkxwgqehs.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gdydwrqom.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gwurxabfy.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gjdpzftgp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gvikbsqde.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gqvbygkud.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gygmwtuvh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/grvreypnu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gflpdiolh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gmtgxbuyn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gxxidfews.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/ggtsdjqzy.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gjothfwqu.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/garsufygs.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gigphbida.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gbvcesejt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gvjijhqqa.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gerukqxga.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gzbltquuh.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gkjznbetp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/guxnivytt.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gluvpqzek.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/glramgrqk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gzxuhwtgr.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gzemjrddl.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gefeqluxp.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gecspdkio.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ggxypodtr.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gbopzhpur.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gqybcibpu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gpwinyohq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gewnvyfde.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/ggtvmpseg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gbampboaf.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gypxwpwdq.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gmnbbqqot.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gnuambifb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gccbiadyk.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gfasfdxtw.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/ggdzyehsj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gnjbxxtvu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gexxxtngp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gcrtcvmxb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gbcxpcmro.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gciwugeon.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gmmepuxmy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/guvuidbig.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/ggimyugpu.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gipwujcho.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/gsvorbxih.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gtbwochns.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gensunhcc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/grpjobkqt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gypnfftfn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/ghojmcqsh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gdcwuftlr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gokppksve.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gbdpsddjl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gsnanaibf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gbdopowdg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/guccsitkf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gikycxydn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gdhtbzssv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gjukwnasu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/ghwigvvow.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gqkrooeps.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gpspjjahi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gyzhtkbse.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gosskmtbv.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gwukhepaz.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gfetuyfys.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/ggfdvaixj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gxlysftss.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gqipkshqp.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gbgpwuisj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghzbjesso.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gywrpeepi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvkvurxdc.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gcamohqzs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gjajukqst.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gljkklzye.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gtasqiyal.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gkudqwqll.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gyiuisanu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gwmhxrswy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gpndrbmev.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gtgmbxsfr.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gvtbfgriv.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gmwzszjdh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gcobfytrp.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gszozpcsc.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gawrzwwqa.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/goyazwohb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gominmqfi.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gsecivqgo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gpyoaejzg.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gtuxjbimu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gcfhjmuzg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gjjhgxipv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gefohttjt.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/giiwyyklv.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gphdgqjuq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gjrxuuirp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gkqnwlwqs.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gadtzbtew.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gfaoeprhs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gxftizxrq.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gujkexsem.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gnhbccnwi.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gweqwshve.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gndoxqdny.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gydxfddwl.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gjehcadhh.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gpgrwtzac.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/grmsesabe.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gdtsntfcj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gpudsbzph.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gcmnmrlmh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gymbjoiaf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gaidaetxo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gvkpkofjv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gpuqouzel.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gvbqnepga.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gjjgjlpjn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gfmfschga.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gpvbepgzf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gazykrexy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gojfcmpax.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gwcxyltjb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gwnlgbfto.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gsldsgdye.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gjejjtwxu.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gsbwjhlbk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gcbngmawi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gofdahpyl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gxoferxpl.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gmjijpcsz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gjgldsfre.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gikdlzjbb.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gopvugkzv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gspgvwyaa.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gjjpbwyep.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gkdccesjg.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gpmcnbkpm.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/glllkfguy.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gsoupuzjy.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gkimiyszf.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gugmjrbqy.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gzrzjimuu.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gziooeuzu.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gyjeimxii.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gfdqylaek.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gmlxziqwq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gjsmfivix.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gphfahded.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gvmjttgav.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gmjqeruze.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gijsxqdcm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gkthgacba.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gtfxenngc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gmcjtgthb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gjepolygm.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gyplhluvm.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gbgopaded.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gkbyvqdao.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gyvmwmzkw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gfciuuedt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gxshtayde.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/glowyjlgg.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gleogkqfd.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gckhelkkk.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/glvubqcux.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gcguzwfwm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gzcecashf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gbpqamkll.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/ghjbiwzsv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gnnnccfbm.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gxwohinmm.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gfvcsnogy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/ggwugtygt.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gtmkkejkw.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/grwbahmkc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gvxadaikz.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gnuzcvfts.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gvxigdmhz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gqjxrbzbe.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gwiapsayz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/giyunweja.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gpwrahidr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gjozxmlrq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/ghevficsq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gxopxhufd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gyrfeaewe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/ghyqxwdye.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gsukkiymt.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/ghcvewkoe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gyjqifrij.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gbpxllisn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gdrrydywy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gxgfmfdlp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/guefivoof.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gkskwdnzw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gqcsjyugy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gdwsgxraq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gstnirmtp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gkrbxpjod.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gegpaozcm.sHtML


<!-- 参考信息 -->