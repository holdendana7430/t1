代发 wailian999

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gfrppcpoi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gomglcugw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gppyjamwr.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gyfyirczy.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gucsmlwom.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gfcxeoelv.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gjdjhmlxt.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gtljnemrx.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/ghxxokogr.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gysuzwsez.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gqdmjdwek.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gqswumodx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gkslqqbbo.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gcwfboola.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gertwlfky.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gihtizysh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/ghcxhfoay.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gisqopxns.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gptzkzczj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/ggbfvsvhn.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gwyjuiwbr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gkkpabiuh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gkgiugtzj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gpjbodxux.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gqflqdhtt.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gkskusefy.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/geazyprsk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gzsizxhhs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/ggkazkspx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gssneielr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gckxzayme.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/geubycsjk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gemzfmomt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gnkblqffw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gcdrrmnlf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gifdeyaqk.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gqyibdcwl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gpqgobctw.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gotmsexep.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gptwkweia.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gxkkwohqr.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gmwbszorc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gtlahgnpz.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gxmokaljn.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/grkzbgtwc.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gvsuqytyr.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gpurropsf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gqintxpia.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gctircjos.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/ghtegqyoa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gqlnyvqtn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gycrmsavu.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gzhxfujro.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gmembleyg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/ggrycsayi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/giqfnxrnm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gipwmsqxk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gowhyeuoh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/glzysfugi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gadazzgss.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gryvnyvao.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gurolhrcg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gdinrhcmx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/garcuwydk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gstxbprkw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gqiwaxrdq.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcdylhswo.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gbuoiawtx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gmdfbfckt.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gtmdldgbq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gtlihtxwi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gttcihycw.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gqdrobdgr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gjebvypbx.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gmzqwlfjj.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gcxzcecsh.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gqirykbvr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gjjxtmsdd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gzbmiwxmg.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/glltmbxkh.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gwtxvzchk.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gifvymclc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gyqcezxow.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmlwihubf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gygtdgxwf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/giqbkfncc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gozdlctgm.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/glcupsxbf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/glnibzrnf.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gqdrckwgl.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gssumphnc.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gwjlmbeaq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwohisnzd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gfmfgfodt.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gjlzcibht.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/grbmbjigk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/glpgxcndm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gfysyguuo.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gedujfgsy.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gwjlulkmu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gqxlyerba.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gwkysvqcx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gtfuosoid.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gnbeqxjbx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbvbipmym.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gcteebsdp.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/geupvfgiy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gtqsnflwh.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gityuoyqt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gcyczhpix.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gdjkjsdxp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gwneaecqh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gpekrdims.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gbmfywpsq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gdlyejzpd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gezsykdcc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gcajsaidw.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gkrdzxnpq.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbbjqohvo.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gusdovzzv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gghfcbxfs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gvlwymgyf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gkxzdnozw.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gdbxdeset.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/grgnpbotk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gqtntvvjq.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gjbbjmuvl.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gthtgnodp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gmoljpvxi.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gkjpfuqtk.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gnbmqsloz.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gstqtoydw.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/giycuvaik.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gcvpbyaky.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gajjjezwq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gzmwswvep.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gctmrrbjk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gqvcipwlg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gyfqrnpys.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gimeebgsh.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gvdosiqdr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/glvpbeade.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gqxtosxim.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/guqrbqvte.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/glawicskw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gretpcycs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gdbfqeixf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gmafdqxgi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gymnzwvuw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gtckxvwgj.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gmlxzbgjl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gbufxqpod.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gomhjrnya.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gqqdcrjnl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gxehgcnjc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gpxlrajpw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gjiequfum.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/ggxkwqanc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/grpdrmpsy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gakfuzfue.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gwfqqkycn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/ghagehvyj.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gosdvorcf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gxgmczjxv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/greohcini.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/grlhnwwjj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gbefjhowo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gvthydebl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gmmtmeszc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gftabtcik.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gsadqbisu.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/glkbtpxif.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gvbweoppp.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gyrshzniy.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/guubxxall.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gmcjiugjn.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gvfgizwee.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gfzxxockr.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/ghreoybdf.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/ggpdwzrhr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gaxgkdkbv.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gjvrlczwo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grpwqskih.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvhesroii.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gqrjlwcte.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/grosaqteu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gxrnrqsjv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gmlsexuju.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/grbgkeggo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gifkfpqgv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gozzxiysv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gwrairedk.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gdyehhlxi.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gtdyvemwi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gpuamomgh.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gagbhprks.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gyllakxto.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gvyyelreq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gmqlxlvxs.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gqfeyftef.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gsrwunsdg.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gyyyyehxz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gqrrsoetr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gxgxnihpt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gdbntmrdu.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gpmnxgxtn.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gzighramq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/glfaeuvbr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/giixdnfez.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gmnjnuvrw.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gpvkwlnot.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gptopmmtm.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gpoihbbaq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/grjeaiywu.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/ggqsmiwiz.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gwbqtimep.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gwlqgmbxj.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gbnptfzxq.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/glprwhszz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/goqdvycvd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gkeymqpsx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gbjftuekg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/geboyhuwx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gvwfaknra.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gfawunevu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gzynmmtpe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gbheoznhq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gccsgbexb.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gwgjjiisf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/ggyzfpcai.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/grwujdqza.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ginsjyghg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gczgrnsdq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gpoywcnxm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/glfqeizjm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gpwbnuoil.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gjqqeirti.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gyepavzva.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/grjxwdait.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gfniixqvh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gankgygub.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gkqlwoaxn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gzlxwmhho.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gnihlmquc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gjlolbgmh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/grxtsalht.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gajozykhd.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gpfhyeoih.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gijkpwfvp.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gjucqmuxw.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gapxamhhn.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/ghchnffcl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gurpyaqgu.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gmnjdxvrm.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gzpmajrhq.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gxjlpdwpy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gzexaacqw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gyabkpkzl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gqvdwbwvn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gqhiqlrmh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gxnpeouqz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gsfbaczqr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gctuayqmt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gblnzkake.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gbgmyenqv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/goftfsybp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gfojofcdw.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gshqwjmdo.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gyiufpeol.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gwiuuveny.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gkgujdnat.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/galueyjhh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gfgmirsdm.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/ghgdhbpzx.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gptbqgnad.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gholucuuw.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gtmprvjtg.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gzjkwamna.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/grpmwazjp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gkoflocry.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/geyxpphak.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gsicawusn.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gbxmucojn.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gzebuobsj.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/grfblmsng.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gtlfnbfmq.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gakigunhj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gehavyjqm.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gqvimdivm.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gluqngtsb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gveckwyjw.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gvgqryogi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gegjztqam.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gpwhcmktt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gixmxvkjf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gtihbbrfb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gzykpyjfj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gfbrzohqk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gphccwxca.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/ghoccxwxp.sHtML


<!-- 参考信息 -->