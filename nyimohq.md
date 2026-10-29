代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gqclqjbtj.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gvjfgrcdv.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gdfohrrxq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/grxyissgr.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/galqwnosb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gxyrdzoyw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/ggbngoefb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gkvvmulhp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gjovydkxm.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gxgzfotth.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/geuctxoma.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gftmnivtr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/guqslhpcm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gkiijvxyv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gljhdkquv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gfmqutyqz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gbaltueyo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gsfhuqdyn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gkgsvljci.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gnbnepfuc.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gyjunorid.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gxyxnesfg.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gviirwppb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gntkcjaeo.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gwamjdwmf.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gojkwlhll.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/glychwnvf.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gwavvkybv.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gmdzlnole.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gmywpexbx.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gwbixvqhp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gaibzhwmh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gxrdpcxad.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gywkdnicj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/ghwzrassg.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gtnuotlqx.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gavxrsemt.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/ghqtwfkwz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/ghrlztmnb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gmniwzmnv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/glmnprtwf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/ghothpcse.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/ghuidjgvh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gehflatpg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gtnzzapfu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/glkqhtziv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/glhlmplyw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gbbfkivup.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gqztysibe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/ganlrbskz.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gbwugadeu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gjxkyxbqb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gcqqlvcyc.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gdfeyxmaz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gupcddtwv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/ghuagjrbj.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/glcdokveb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gcthrckgw.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gjbkbitrh.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/ggglqidgf.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gaqdrgmtv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gmdxdrlze.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gtearprph.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/guiohwnfy.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gddgxbyeq.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gjocfpdnf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gjcuzmlmu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gcupuulab.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gtvungbzw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gpdmxxkhg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gcythvwsg.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gszpyccna.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/geliavyly.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gusqhnjfd.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gysnghuhc.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/ggerqlbfm.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gvrnikmrr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gjvuurpux.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gcuyydsfr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gcffizhtj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gyabnkswu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gcrcdecbj.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/godbglynl.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/ggzytgrgj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gsrtpkako.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gnziedvov.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gxjzjtnzl.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gdrufmszh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gniesddij.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gngwmjekt.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gnqiutkuk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gxwngqdam.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gpintotbm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gnpsksajm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gqqpochlh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/geeduraqq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/geyrmqtlq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gogzqkxyg.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gfunojljw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gigogvbtf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gvomduscd.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gzkeaukzk.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gfcerowel.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ginprlnsm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gqrlfxnll.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gzrcrtzpf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gemajrbvt.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/ghyzsqjdk.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gooowxmrn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gwjhenwjo.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/grpprjhrh.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gizhrzoul.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gnybkcfgv.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gvbsvvmcq.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gccxivghn.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gfimkrdyj.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gzwcktmke.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gpmkvlxia.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gznssptxi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/ghjlprrjn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gxxhxssgv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gvzyhkkcm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gymyzuxoc.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gzdjsxtdd.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/goeenyfse.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gtmeiaeiq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/ggtulobje.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gdumtlmfb.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/goirvfzaq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gtlgbaffb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gwoynrtfj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gezunyhaz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gkmygnysb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gmziywohc.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gdhbvmkur.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gqragbnng.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gqwejdthy.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gtgxfngqm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gjtxfjzjk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gplelkdrp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gdtpbrsgz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/ggyloausq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gbiflekwi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gounxtfra.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/giyecoire.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gxiiqfmjg.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gsrrtkvon.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/glivxvhic.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gaotpgmhu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gqnqycafd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gdtktshxv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/grjjkbxbx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gbvgrqshj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gszvlegxa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gcpbzungg.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gregxzcox.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gvobpolhe.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gveytejyo.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/ghmkwrkgj.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gwokmhmev.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gedovopkl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gbssadfex.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gsrtvtixb.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gvyylqaxh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmshrhaxk.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/grylvjngj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/govjenplc.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gpflwmwhl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gzapoqqro.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/golqiblhm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gumbdpqtp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/grtmkluej.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gxchhvyfn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gdzwphgam.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gpjsigbxy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gziebtyhi.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gijsftxfr.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/guixdnngm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gojrrylny.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gagqjokel.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gdjekayyr.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gwwkhggku.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gnwkyhdzf.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gwdsqopch.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gruiyznai.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gfysrplhs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gvbrufuyt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/goyhgwdza.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/goiaszjcr.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gxdoxeeff.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gakzinnrj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gbixqlkpk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gwiofmsjw.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gnkyygcvs.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gezntepwk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gayfoliim.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gyirkmmsw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gyrnclhve.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gfmfarkqv.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gzlsfnwis.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/guuewcvda.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gtzpnntvf.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/geduzfsvw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gpwiefhkd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gxmivvsmb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/ginzkcygl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/ghraghvxy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gokytuuin.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gtuwfxaah.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gkuwyyjuf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gdwmtwfhv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gzkandgmx.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gfjggetse.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gbsktblml.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gqrvrazxw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gvyuckxxb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gjiwkfumv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gzkzrjyxs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gmkmvvmxd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gelvdnlft.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gphmuxfux.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gftsvvfad.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gprmarzbk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/glsereuvy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gbphmeekt.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gqtumiwcq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gpciiznrz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gmbtsccfv.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/garysubks.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gnksaieto.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gjpssprgo.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gvdgrtzev.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gnbcdhqwt.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/glhduiswz.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gjafnugrs.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gknaapkcc.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gwdsjvvrb.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gjljzrgla.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gejdwqpei.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gmockceyi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gwclqzddc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gjhjcrpnw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gdeuvhqip.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gdrgqszpi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gxqhfuzsp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gcrscfzhl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/glzrcogqa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gfjyubfkw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/ghsvzkmcj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gfimnznxm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gpyistacr.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gdrvhlipw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gfojrocoz.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gqohdmevz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gegnopywa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gcshjbakq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gtuxjncpr.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/glqwycnue.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gwgbcoyas.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gjedqujrq.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/guupwtvcv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gahzasivw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gezbwveee.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gdcmzitoq.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/ginkqaqwu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gbxippkqy.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gipgantnd.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gpyzbptqp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gvsfsddaj.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gidrrloci.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gbrbyrxex.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gneuwdvjj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/ggfwhbvfq.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gyktvasds.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/grfhgibsp.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/ghpdelzqm.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gyxffmbbm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gkjfgmras.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/ggcxpmzba.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gohqdfong.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gdnllagxd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gtzpzfegn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/giunfcssu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gammhobsy.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gditektjg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/guzcymtem.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gvhzbrdvl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gyfhredfu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjglqyfur.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/glhwhhvob.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gjbgizzii.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gtxjqdsva.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/grjxrheqn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gjxqpxppu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmzhopfoi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/gfjridqno.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gstiaomxo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gsadxvonk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gnwvggcno.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gnrphlvyx.sHtML


<!-- 参考信息 -->