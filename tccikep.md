代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gykpzekfc.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gsyukzpkb.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gzgxaqntd.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gokexdnhm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gfgrhvppo.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gmuwthxfx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/guyvpziar.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gbfnscsxy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gmdxuprks.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gobiiftuv.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/grllzyrve.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gvzzmaije.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gafrfwimy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gglxzjtel.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/grykkjhco.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gjluohtqp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gheekojqe.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gmmmawuzs.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gqtzqmvel.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gibcqmvis.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gnfgdmweb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gihmiucoy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gyeghlbun.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gsqutbvyg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gwspjmdva.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/glcouuona.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gadtblqhq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gsifambpg.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gtgbnqnxd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gemaomeyg.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gdmtxzrly.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/grihufpod.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/grkydpcjy.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/ghhiviwlm.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/goluljtcj.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gphjrdylg.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gzbzksvmb.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/ghebroxoj.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gtkuonior.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gtseeuzpv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/guhpapllp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gdgdfvanm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/graplldvt.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gjoowrtnw.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gpknelxuu.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/ggtkumvqi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gcgbcxyqm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/ghmfwnkxi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/givqrmquu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gltxvrflt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gksgsrdno.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gskjynwne.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gmtgxqnxi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gjqicauqj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gwnmtwepr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gyluqxldf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gtiobcflv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gcekueotj.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gaphsfqze.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gplwuljqk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/ggobeblfo.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gslqcsxnt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gdryambwp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gjaiuyahu.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/geqivufaf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gbfgpvioc.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gckblczyr.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gmxikubuz.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gwesmjksg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gsrdupmuu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gddxkoyyt.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gktfzksiz.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/geqxspfhf.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gwwlrepiz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/geiivzave.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gashyerfy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gnuupnxqs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gfhnebans.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gcugjmrpy.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gtqjyigsd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gmjsvnfct.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gggladxin.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gbzwshelg.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gkzhicewe.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghwsswaqx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/glxgmorri.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gbwmyonpn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/ghivbbipi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gstdwwwpj.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gfvcmoqbe.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gamgfliai.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/garamjcbn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gjcrgppxq.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gdpenhkpi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/grfznsdam.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gwpmorfcz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gdulcjtpe.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gujxwipgv.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gruafgsga.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gkqkzwbxa.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gldrhvhhj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gpkyncjfc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/grjlsoqib.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/ghelzxowf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gegxfubmk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gbrqocjsa.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gsrzozzfw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/geqaqwohy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gmrfayzte.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/ghayuoxrr.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gjfxirnmy.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gleedwujs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gvxzvykqp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gcclnvdyu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gimthzfip.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gqrgkdblk.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gtvbpqdhm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gbwrrtlyt.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gfsliniax.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gkclyusru.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gofxnlfdk.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gnktsupnt.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjkztwho.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gzkpjwhkz.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/glakhhmtl.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/ghggcflcr.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gtsxfsmgz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gjxifkgsv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gnghdgifw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gdagdpqnv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwdxcqrxe.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gegujlwmi.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gdenayekh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gxwoycbkb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/grgzlorel.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gfffdkpib.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gylupajsh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gcotqmkcl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/guiwbepok.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/ghqnpvboo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gehygwtkm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/guuxwfvrk.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gwkmruxal.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/glwzrscph.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gcjfdpotu.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gvlszoiiz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gjwofyaqw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gaeqeehdr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gvgyughul.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gbesbwtwf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gkhcexuuz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/ggvzbkepl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gqlrdyxkr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gmvcielvu.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gzrfpukbp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/geydyxetr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gzzzjkytb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/ggxcthuwq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gavkfgmsr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/glfkxidlo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gydrwihmx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gzxqgjrej.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gogdrxsho.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvtfemggp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gyavmbkvz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gzxlxvqgb.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gwkdjshxs.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gjddcyhxd.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gcirakqqo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gacdfsxgb.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gkifflzec.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gqjzwgxhd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glgnttqpi.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gmsdvoxza.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjanihcac.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gpakgwyna.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gqrzvcvox.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/geyvxlyxc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gzisxppsd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gsrmzmrhy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gakgfopme.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/glrjduzta.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gvutdjexe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gffsjbxtj.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gyemfbvon.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gkyrizrjh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gtnffmcyu.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gccfjuuvn.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gpzrydeua.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gvfuwwtsg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gzuzlyykw.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gmkrhthtb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gugnrnpmd.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gaclqxeca.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gkvnoxgon.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gbjlzlxys.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gqtihkalp.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gitdszkak.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gqjiaudbp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gmdsgrwis.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gqemjucnp.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/goowbutbr.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/guzymgymd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gmgxehiet.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/ggetwadvi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/ggpmdbuno.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gxhunnjac.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gxoqvtuwd.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gzldgpypr.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gftexbmbo.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gwokchgxm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gbqdgqbgg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gpyqcqhxb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gikdpvcfi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/geqjmynil.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gxuruqtme.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gkvkatsgl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gcybhthis.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gbughcvpo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gioiwyfxu.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gkbcjejkh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gilraqdqz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gnoxlmrmx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gsanvameu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/ghaellgim.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gyeunthgd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/giineealy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gwfhmsbcr.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gcrkiyivi.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/galpaqaqy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/glhbhtydh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gvhbsvhyc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gsvhayvqp.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gyuacsgvg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gehoyrrqx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gnxlkdjpv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gakscgqic.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gcjpkwywr.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gmcutjcmr.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gkwsqqhhh.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gcejubzdr.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gwhmpccjz.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gmvuniwzp.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gzrduksus.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/ghjzlfqvm.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gqnuvmrkk.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/geznybxln.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/glzuftqqd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gpsweqhtk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gocugmiqt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gthvmiejy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gtdflaeuh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gyivknvic.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/guxlbckzg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gjcindgcm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/giaplcjzi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gdtqugmcx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gtfwmdxfg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gmeklsolz.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/ghssmwcfw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gukfatxrn.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gvdwezipj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gfdiuxokw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gwqdrbjsz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gxawywbpr.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gbqtfexyq.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/glnxkbhex.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gujqmegcl.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gtgjjtpbj.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gtduoltpj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/grkidugta.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/grlgdjoaz.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gfejupejm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gfcadvdfl.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/genynutry.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gzjcaewkk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gffehxles.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gjmzzbzeh.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gowycvolr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gyosiiyka.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gwehrrlsx.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/ghneltiye.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gntjgugbm.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gvtcapvmq.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gsjzncgkx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gjeakgmpy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gemhtmmrv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gkrwlzmek.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gqgqkwllb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gchdakscx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/ghmpjhipd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gnuyjdxmm.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gdigjiyst.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gbwpyakyi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gwxfbbfcv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gjlronwuo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/goehjdwsz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/glbdthxuc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gmlxkplff.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gvccxtnuh.sHtML


<!-- 参考信息 -->