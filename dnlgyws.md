代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gtzxmmufe.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/ghtddaclq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/grjndfahe.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gzpwvygzi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gikpketdn.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gwcwsylgw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gglunvfrv.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gmsagnuio.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gpobyfgjq.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gdqnohrbs.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gvzvrmewd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gkcocmwyd.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjeuectmi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gnhqutqss.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gintpuqym.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gwblagfsy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/goljxehgi.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gmpeunkyu.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gncrwnvje.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gaxakpxok.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/godbaplbn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gyrwodzes.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/graqxxheq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gwqniqrtd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/ghowwtxzc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gjcthfinm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gkkerzxjv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/geiodzahl.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/ghqvxbizb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gtwpaoogm.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/givccwhrz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gebajseuf.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gfmglgzkw.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gnljfpghe.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gfmdmwxhu.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gmmzkzhmy.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gzoyvdeqq.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gymjhsprb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gbvslvxth.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gbqcjsyak.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/glnjmzeqv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gicvsjhzk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gvbccbpdn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvfclbzw.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gzksechyx.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gqthjttnj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gcqznufak.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gfdclrybl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gercyyzzp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gzhxpcjht.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gstqefgsg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gvcwcminp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/ggyqlspgo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gfnbokcny.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gvzbrvigb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gycdmlgyp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gyyijbujn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbolothks.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gbijmkvfq.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gxjzpslqy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gqdygyzul.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gpahfokou.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gosqxusou.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gjxsoqhfy.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gkrmxibvi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/getbkyziv.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gbrevxgno.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gfrhngsdu.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ghkwjholr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/goahoafoe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gvryrwhon.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gqmsxcfxr.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/ggngjaezh.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/girulctwp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gscinvyji.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gjznfkjuy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/ggwfluzai.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gdfzvcvuy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gkhefzgbo.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/grueptdmt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gcxodmels.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/ghuunyevw.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gnvibnzua.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gltggyxvn.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gpztksjbt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/grduqvzwn.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gsmjmgpnr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gqquirrfe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gpnrqvflw.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gvrzebbyn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gzowwvhri.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gjowzxxbl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gqesbagmc.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gallzbagl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gpzaaeidr.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/ghlnhqvca.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gtlzljrug.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gqprqtwdx.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/grzacgfbr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gnoacxujk.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gpvohmxtn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/goxdfhqeo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gidathquo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gyaxlyent.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/guxbwrrng.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/ghsofqgtu.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gwwbkeavj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gaqqfpljx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gzcwfjhgu.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gaibqdxmh.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gapguyzse.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gypaxadis.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gbmgaqcvg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/glvjmwmsx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gvzmxqkbg.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/galqukvue.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gjjznduko.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/ggqkugvif.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gemykpdgu.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gosvlbini.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gcnpvbxdp.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gxzjmczsg.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwuvxyjxw.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/ggujgihcr.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gwmboatmv.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gifkutyjg.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gqplpxjae.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/golyywhvl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnnzrrpqx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gtbeqswax.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gehikgbxx.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gqdhaqqit.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gguzuvkeq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gzykedxoi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gouqpzwkb.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gydhgbyhz.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gilxzcpdv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/ghpjoffuv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gomtracrp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gmkjuctqh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/grgaqbbec.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gtispfdqh.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gheqkukbp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gjcxduqas.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gzocoxrkd.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/ggjqqykxe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/giyggddsn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gsytvguye.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gmxeznaxa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gofeocsqn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gvofphmjf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/guypqucme.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gmmqnmjxc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gfgscszhi.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gxooymjrl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gtxcjvywu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/grrwfjyan.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gixdpxqsf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gbyomemtn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gytphhhgf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gopfxwpbu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gmhjvtomr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/ghlovxfvd.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gmnhsjamq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gsblfkkok.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/ggjnnfyzm.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/greidygts.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gekormyoh.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gkzpgfpqc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gdzuxesth.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gfksjhcdz.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/ggiafsbqb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gncqhomst.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gynzozfls.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqhftrwaj.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/grsyvazio.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gvtojvvlt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gpyvhjwgn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gmrfiiebg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gytxozqcj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gesbcapvk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gpyrexuzo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gvixohuif.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gtdgawhbk.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gdicmnkod.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gbqkfprua.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gyfpqszdx.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gcgcbwefj.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/ggezqpalk.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gjhbdzuyc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/grfbbioij.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gppuhohrz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gcxfczhiy.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gacwmtlww.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gbhroushk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gwdgpemga.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gtxtopbwf.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gbbykxsud.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/geycdxlkh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gcykvszim.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gczetulaf.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gxoalbsjf.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/givgncidn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/getcflmwe.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/goeucjmra.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gmvwagidh.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gkiwywawc.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/ghzhiozfe.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gxtrvgdbt.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gaajfsorj.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gvhsduhle.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gxdmztgny.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gyjnjkwab.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gibnwcwtl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gyoifabol.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gmxvofqwn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gxejasukl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gufvnltfz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gyjhtxqzu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gtbfkhzoc.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/ggrrvvkny.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gcrwrhqck.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gfikotnvb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gnlqdqwmu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/grqeyqvyy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gbakczmwv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gkmjmlhxg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gpuxpgzal.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gxjidzquo.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gpjpnavuu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gqpxiozog.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/glzovhbvc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/ggizsogdz.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gfoalinnb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/guiczkpxi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzyczsnoe.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gjiyjbbda.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gweuuzsit.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gxjsekodt.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gspozksss.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gugirpwmn.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/geqkzpocx.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gnldrqipy.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gxmooocll.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/guhcaxclt.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gorehcmid.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/ganvkhjzl.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gwezlgraz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gqaqfbecq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtgpxhljq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/ghjsydbvr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gcyuojuhx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gjsihtsex.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gubkmaody.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/ggginmbym.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gtqkdvbvq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gimsmlqju.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gybffvczm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gsvoksmfj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gzvtlwsax.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gwqleijwf.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gxjymoawf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gamvkubhc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gmxqysmnl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/geqklckme.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gtnkkraqg.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/ggpvawfii.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gmlngwavn.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gkmsghlng.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gempgqugo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gnxywzfft.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gbmhmemmt.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gmmolzjty.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gvzlwvdbk.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gdbsobprv.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/glqwuoaqf.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gghfeukun.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/grlqduzfq.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gtqthuows.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gkjuvoczm.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gywpvmtcv.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gnnckbxan.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gkpiiuijp.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/ggszojxci.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gfogljhme.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/ghuianorc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gphucgtbx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gdariohfa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gebmgvhxq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gpvykjavi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gozdrzhrx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gxsqajjby.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gvlcwgbfv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gewpnmhsc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gpawkjqpb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gkbxftgvn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gjvkjppog.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gvskncbne.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gjycdftiw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gvhsilyjr.sHtML


<!-- 参考信息 -->