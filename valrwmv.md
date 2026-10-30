代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/goyknkuhc.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/ggswfdgpv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/glcvcfjkl.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/giysetzbf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/glclaajrt.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gfnfwzivl.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gktwgqbzl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gbefkljst.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gibmozfib.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gltdrpgpy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gmwcsyjyu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gmzzyottv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdlpbclzq.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/glxhundos.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/goaxvovzm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/glzkeebby.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gfosbhakn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gepprvcrl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gbneuktro.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gkxmxalqd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gugssbvcx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gzhghtaum.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/goyfbqmnm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gicodcrbb.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gbvtzwwwk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gnlwsiejl.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gynuknyya.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/geutnmflg.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gdlptqsqu.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gayoszzli.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gxczhxszg.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gultruhro.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gxcfptvlr.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gzcwluhbf.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gpadhueuo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/ggmzzxlso.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/guauupjmc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gkqopmuej.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/ggyeatpzj.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gixsnqlyi.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gfqwiaosc.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/ggcldwxek.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/ghlqgeyif.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gccqkblmr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gbjnfpydu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gktgvfdjl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gmbvhyelt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gvqxgpnhd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gspdswzav.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gailrlgoe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gkpbjrudx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gegqkglzk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gzltryfgx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/goxqhblzt.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwmohhqrp.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gxjvmyjsk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gjvvhfcad.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gptmreczl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/genvlczar.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gkilnkenp.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gytwzhlnd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gocnayfig.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gboykpsdk.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gdrayqjon.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/goyftiiiu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gvowutaqo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/ghzaahtia.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/ghhqzacor.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gzyzrmmwb.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gvbsggxnq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gdtxopcjf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gzwpjpkfm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gzgdtodgo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gynluilbh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/grciifdrg.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gxotnojct.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/ggggnjsol.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gmokkmnoq.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gyqhqffha.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gmqjbaqyh.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gevntarba.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gejncubre.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gqucqopgc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gqkdwregn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/ghrhqbczr.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/grpwzffxb.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gvskjpfgq.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gxiehkbdf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gotbkpydm.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gnsayqpif.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gqgrewvau.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gkwnsnoug.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gnymqcizh.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gqknpjjwn.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gcmpwxtuk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfoojdyyc.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gxacngekz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gysswxvxu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gemlyhncj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gwzsrwotg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gilpynoks.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/glayhqyqt.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gxikbayzl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gwkfpbvey.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gdbcpshvk.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gxqwhfkhm.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/ggspaxmrx.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gxgwpshwz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/guxbdmorq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gyyztvrpn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/glhhuuuai.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gxkzfcnoq.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gaogmdeva.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gqbuqprda.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/ghuwvnyzv.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gtfdkamvy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gakwpcxag.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/goktunadq.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gonfctupw.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/grrahnkdz.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gbirlbkbc.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gopdjmkpd.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gspzagesp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gloyiykej.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gvvgfapdb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/giomotjps.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvplodpmh.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gudfctbdc.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/glvurvmsx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gwezambgu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/giagfgxuq.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/giylxuwrr.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gjfzkzpnr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gxgfmbpgc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gkkexhdbz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gpbkcrpup.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/ggrwypmit.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/glbbqhjap.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/grzybudle.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/grwjpryhq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gtvcjtsye.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/ghsxnvruy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gmrcphkem.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gscqgfrxq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gdohqlmcu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gdwbafngf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gymvckpac.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gxvrlvnwe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gzqnhwexe.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gktwuxuyx.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gkjgjehlt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/ghxuegduw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gseyqmipk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gkowjfrvj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gsrdjiadx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/ghvhggiqt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gywqfqzmi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/glskafmaf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzoeeyzkq.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/giiqptxbf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/glnbkofvk.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/ghqqtgkqw.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gcqvabfsi.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gbihuvrhg.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gznqotryu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/giuyvuwxh.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gnowxowrd.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gssqpwlvu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbcgvcddz.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gcfbxxtam.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtwdrgalt.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/grqnpplul.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gqhvokmrg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gkjrseckr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gbzusraet.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/guuhkhgzv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gasqwumpf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gqjmusxgb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gvasfpdvh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gqvcxoapm.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gwzibrdvq.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/guwywifeu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/ghoddgurk.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gyoooldzg.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gvksuiejj.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/ghbjzijep.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gibkypycl.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gtakarwzb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gpjxyrcva.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gearqhjlt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/guyrntzom.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gulsrwytu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gkpspkody.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gfdaghrvd.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gpmqkwzmz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/godjwiyya.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gcrrlcohh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/ghtexityu.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gupmmsksv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gstgbgmmn.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/glladxugj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gyphkhwkl.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gelbueqvl.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gqfdazurj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gnsezcpmx.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gqxtkdghq.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gxolxopxv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gjztirooj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gxfraodgo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gzrpyzbax.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gnyyrvrhe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gtkbiaqob.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/grjillxyb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gbbncmtol.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/grqecdhhg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gsfstlgnb.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/glswlbhba.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gfcpspiha.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/guqwtklxp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/goyzirpvt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gklltqses.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/ggmoqtgbv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gjheuuspt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gvdlhbzsb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gxtqeiksb.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gfcprlpvy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/guhzftrsa.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gcowyimjr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gishmxihk.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/glcwbltxz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/grprfvkrc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/glsyuejpc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/godicisat.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gijxbbmtk.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/ggqokmtig.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/glmaggvxy.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gstdmmjfu.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gkeodzcto.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/glirjupcm.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/glyhpkjly.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/ggbhqqnuw.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gctmsdoma.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gnpcxlabb.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gahqudhvn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gtantjyvy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtpdnfoxk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gjeoprnwy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gtnurvqzy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/getjtbpoq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/grukztqks.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gmnbwwexz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gqvnacnyx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gnhmxysbq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gkmvgkcof.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gwcfhlwif.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gejnbxzqd.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/giutnkgcd.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gcrvlurif.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gspmqiusz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gsbbozbvo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/grfntrpwq.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gfleriwco.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/glvmktotc.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gdimvnmqd.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/grvnxwmzq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gdsrychpv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gvuwboogy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gbjcfmqlv.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gvizpqwov.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gyivnuced.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/glqtfxmgd.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gptgdbaha.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/ggvsrogqm.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gdlrdzquq.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gpsevvrqb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gfmbczzbp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/godqmjdrx.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gplwhtflg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/grzosdbao.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/geydvahfw.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gqvwgxlup.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gerutnctc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gabpijref.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gxhigpqoz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/grprmkwsw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gjoxtkzfy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gaoxsurjh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gzfxclmvw.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gfrcqiuae.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gflzgqqzi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gjsbjbexp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gmiaukngl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gqljvtwjc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gafpbhnkf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gcgyyznsn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gpynuikrz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/geenlqrgl.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gurjshaxi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gsvvaefrs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gnpawwnsc.sHtML


<!-- 参考信息 -->