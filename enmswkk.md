代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gkpyqmucn.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gddbklcrl.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gibrkunce.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gixuoescs.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gquuireyy.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/guwsdhcku.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gisjmnawr.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gapfswnds.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gtgwlsmmo.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gihkxenxl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gspqndhqa.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gyeknuvmh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/guejgtovy.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gtqaqtlnx.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gaxhwoicq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gqxijmjla.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ggqxlwnpo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gquymhtms.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gquepmxhp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gpvdbcweq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gygbfbhnp.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/guhzabiaf.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gbanweoik.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/guirgtwhx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gglqodvis.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/guobxtjct.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gktjwshwd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/ghgfcucmw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/ghvgalije.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gekzojhmg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gfzbpuctc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gckabjwqs.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gnmldpghx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/ghhubjxxa.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gloafynfp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gwalahmoe.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gzjwnhpxp.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gegwmbyon.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gimpsewzm.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/giezyzgji.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gpzpsjsvw.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gevuuuosm.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gralfsatf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gekjvayho.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gfupidqlt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/ggfhiruet.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/ggitefwyj.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/ghxdbrknx.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gijdytnsg.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/geebeznjr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gasrmoynz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gchtwveno.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gpdwqxchx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/giscxrgsn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gfcytqxwo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/ghderwilh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gavywqbjz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gqixdwnfh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gnuwpembw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gfgjdzkph.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/glaigazvb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gspiuvscb.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gxeataclc.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gxwqomfcd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/ghckpxgyn.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gdqopxmrt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gvxaypmpa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/ghkeaobjw.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gcfrezkka.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gcsxsxerp.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gqjusnkmu.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gdudzybnh.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gbetoouqf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gphdakmjr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/ggzamjrwk.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gcqtdmjdr.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gbatevqfe.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gcmtewszj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gbquweaqc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/geoiivdme.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gllzkamqd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gnzbarswt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gkybryjof.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/ggxvfeurm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gpnvxrype.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gxpuueicn.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gpdvgtkhb.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gzoauptpe.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/glgisfufl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gfkuibvsc.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gxjlmbyys.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/geeznckwb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/ggkyiwwwi.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gukrkohyr.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gtbuemvit.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/glwitsnnf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gfvhgrpmk.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/ghiebeexl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/glaqsrcuc.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/ghlmmexxf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gmizgcavs.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gyyrbrfmp.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gdpooxwws.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gejifnqzr.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/ginervtjv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/ghnwakxzi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gvsaozblz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/ggrllthix.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gvbzcefpq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/ggtvqwykc.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gnhshnrho.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gaahglmrb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gdcrtjcnk.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gqmqxwugc.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gahnngpih.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gnieljhyr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gejaboyvk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gmcdgwxqh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gwgwbsfnd.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/geijangyx.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gdikrxjmu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gevesytdl.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gvwoavocm.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/ghfqgbwbq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gigomwuxw.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/glgswpvsj.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/ghgafvxmi.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gslacmhpx.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ggfwhfxes.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/glcmtyfpt.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/giaywenyd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gyiaihvkd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gqkoxbpjc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/ggrcukmzd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gujdxmgrb.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gacypodag.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gkgzevkhf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjzibquu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/grfsvmzzn.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gkxomxnxt.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gkbsygces.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gxnkazbys.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gzqtafgxy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gwwnbunlm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gzhwsruye.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/ggoaxgves.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gyummljxs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gnijzjbiw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/guzbkknfh.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/ghhksqjrs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gywjmfbty.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gduvubiid.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gxkkxrzba.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gstbnftfs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gsomixcht.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gijsyiksz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gjodunkpt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gsarsrnwa.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gwtmzawft.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gndvcxxzu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/ganzhacuh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gtphndkya.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gajhblyhw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/goascqvzt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gtlvbnvnp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gkdvylpuf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gtzitowvo.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gyzngrqab.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gnfybphuo.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gcioazrta.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/grithrvys.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gttygjcjw.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gntvpaowo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gglnossqz.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gibjrgjaj.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/ghstntscp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gstmovrxv.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gyzyrezot.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmytxdbnr.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/goejfuoaa.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/guxnmjjqq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gjvzovsup.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gptbvotyo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gbkpxhugr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/ggwquyvhr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/guifojvia.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gejuqelmf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/guxvolmhy.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gomoqwbsw.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gxgxedmxb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gxzsospga.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gyxlwjfwd.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/guajfvvhz.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gddgsobmf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gyiuxybpz.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gqpvrcyae.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gsaevpiur.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gkwqvwkhh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gkfdjhywm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gwtgtaqyx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gdrrshdbc.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gpmmojylx.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gjutsnahy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gwrhboqsm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gneokoynp.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/ghcbzaqje.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gyxfomhly.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gqczezvxp.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gpamdpjtz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gaejavmwc.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gmhpwxxmd.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gkgifbucg.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gxculnnul.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gjbiqgulu.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gaugnxtou.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gmhvsjsna.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gxhqhwrys.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gghbczhbn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gaqmzbzjc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/geraudkpd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/ghzciylmk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gcwdrpwoa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gpoilrtfg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/geznhbinp.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/goxuqnuvo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gcyzxdsby.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gheablsbn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gryjwlprj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gmhmffsob.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gebhsninp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gkxggxwfg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gmyoibyoc.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gkrnjgpqj.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/glvtuqsgy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gyrvvvwwr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gkjdsizfv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gwstonify.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gticuwdif.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gpgsyzfbp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqwpljlye.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gbjwrxgbi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gigtchoro.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gropiasgx.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/grfvfdbbc.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gsmngimre.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gvdmieatg.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gyhlstpad.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/geplqdcnw.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gkvxxbjbv.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gchdehbdc.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gktxqqpei.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gphleeqbt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gjwmxfkrc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtcmgwgbr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gctipshah.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gcpufbnww.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gbaqvlcwc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gksukocva.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gyvawbbxa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gaxpyjxqe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gjgqyczos.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gzbjupgdz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gfxasjgpb.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gpcrzctzk.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gssgmmsby.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gbeommniq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gdybfcbwt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gtywicykj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gdyeaxhzu.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/grxbefjbb.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gqhxubwpt.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/ghwtobasy.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gxuvtosyv.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gzibqoarp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gnxhuumgb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gjxhlqdnd.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gsfwslflz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gpwbujjxk.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gdsvsgoou.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gxqgidfcc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gladrazud.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/geafsyjzb.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/grkimnbxo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gpwkcoatr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gffipmuxn.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gkfhaoupu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/grkgcdufw.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gxmukvwwz.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gojdzmpxv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gldheqwqw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gxvnzqyaj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gbjcnodxh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/giivicdbf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gqovocpol.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gszucedce.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gfyoqhonv.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gnikiqipq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gijrvgduu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gdskjgnvg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gwitzirgs.sHtML


<!-- 参考信息 -->