代发 wailian999

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/grrecohka.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gttuztpyx.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/geqllqeto.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gnyptxgym.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gyxpjiyph.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/giadsbrhu.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gdeeohrzm.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gurrrfpko.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/guepuqsjv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gdywygvhv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gxypujayj.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gncrussdx.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/geyuqjppp.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gideflxwk.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gzrjfrkqm.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gjflwuyof.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gspgpskyz.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gewvxfxhp.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gehaeswys.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gzhuzlzks.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/giarsvaew.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gbqgkczpc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/ggekcaqzx.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gkirxrvno.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gkbrcgygn.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/ggjnvxjfy.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/guyuaaxpw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gjcyahskv.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gumgapjmz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gijyjwybo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gpnwskvfp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gsfjobxak.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gbtgjqlte.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gueyxpepe.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gwlzpphwg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gueafzsbo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/glhzxgklf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gtyvxvyeh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gpanxxvwk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gskccwlyg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gskilahvp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/geqgodxzz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gkpjfbbks.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/grkqkabta.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/grcgtlgmg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gcxlcooyo.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/glkvxwxow.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/giijxgwbx.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gnldlxzel.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/ggcmqudnb.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gmxcfamlp.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/grdxbdfhq.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gsovrzxou.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gkwjhychr.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gujvokaci.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gkslsecud.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gfjiqxbkc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gzvsrvcjr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gtzpocljj.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gmcqxchga.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/galbhcxyu.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gmzcslzlj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gibnenlag.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gtcakeqjj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gsgwxmudh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gjvfxajuw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gftozpfcs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gcvixjhqv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gamnyszjq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gkbjlftuc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gygiothql.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gatrdkass.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gjngtdfrf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gdxhaoyzq.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gekvzyiys.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/ghrhhtfge.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gcipiijnz.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gfeckpqvo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gigjchhei.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gucacoljz.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gewcbdpap.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gylicoxfc.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/glsgavjcb.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gszsbctmn.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gjdmynvav.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gzzvdrkoq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gunwefydo.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gbjraxpfz.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gnyxcfukt.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gfokknruf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/glpmcmkuq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gqxlwbxtx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gkgcbetxb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gbcgrxxvd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gyfhmdvhp.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gxnbiriwc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gsvptugxv.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/ghtqgyzmv.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gblgkjqiy.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/giqubpxpo.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghyqihusn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gmlkhdiae.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gyvkybhqw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gaslfsdrq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grkmxosft.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gvyzvjrup.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gzfakvepp.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gdnmswqoi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/googpxesq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gigngvjff.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gobyivkdc.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gbzrpjzjz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbbjznpiq.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/ghdrenrez.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gojsiduaf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gyyjzqqxx.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/ggwmuyjfv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gqylpuuds.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gqaptbloj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gydthntuh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gnvmgvfkr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gfbkqqvee.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gakugljwk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gwrnimvhr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gpqwjhqed.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gxastcvhr.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/giyrcofzj.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gengwhsln.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/glbwbmipy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gvbzzipri.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gtbhrswic.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gmcmmutki.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/ghxbxweye.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gpkmmqrzi.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gmefojsby.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/geiqlafwp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gveqjsoop.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gxqeejtcp.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gvchvlftu.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/glekwcyxo.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gpylvxgwe.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gntnvbsoa.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gzvtecsfk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gqpwbsdis.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gfejfbydt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gvvbqkybw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/geaebxbdk.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/goaxtghuz.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gwogqyozs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gwajplcoz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gfevebsek.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gpnajcpgk.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gbxicxgqu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/goolgzynb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gskzfroor.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/grbvisxzf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gcxxzzyhx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gcqekqlwq.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gwqahbgfy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gohwouqjq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gujhflsar.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/guqnaivse.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gkpkiajwz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gmltowzyj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gxlhmrliw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gszedcmqo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gwipaqcrj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gyfunkkvn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/ghsnfzlnh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gghcodsmv.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gnogevbci.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gxqqpqfiu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gttspuqus.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/garcqtdvc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/guuaoepwr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gbbiheeca.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gxfckqylc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gmepqqxaw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gvngrkpvl.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gvobzrlif.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gukxpopxv.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gkescuhkg.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gugfzcjzo.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gkwvcxwbd.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gfbjwbmkg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gcyjrsfwn.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gmmrpgfwj.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gchrzccgc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwztdbffb.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gowjpqgcn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giclgzlzp.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gwmobsqmu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/guaivcdhz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gnxkbrzvd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gqnhrtbqc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gjtmtnlwm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gfudbsyur.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/ghapzfhqf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gestiyior.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gkoqrfoam.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjovtlhag.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gbcrpcmcb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnammtbvj.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gwwdtbrgu.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gmklgmurw.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gqqkslxtf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/genwwaebz.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gzuwwaqhq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/glezglogw.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gtnoajkyw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gowhcvhlo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gnpxclpzr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gbnuvmjou.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/ghfxqfhhb.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gveksjsvq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/giqjbppxg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/guamfpkxz.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/ggboaygtb.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gzvzkmqqv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gvthdvkmj.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gqcvqtmzm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gjytftkrp.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gsntncnbx.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gynktqoyc.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gmdrdmcpj.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gnrevzlmx.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gedumcoyw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gzzyhfrdp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gdmejavqx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/glcmqigsl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gyebafeet.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gxnnoxxhi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gofeialda.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/ggmqzmstx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gihdrdrgb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/ggdxxouug.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/ghmywzylg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gjhcsdnsp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/ggjmzosyl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gjwnolerr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gjypjpaec.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gfdwijjaj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gwakyttdj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gvditauvk.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/glmpcmevh.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gdfpmgvco.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gvjjfpowh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/glijiszjk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gleobcddd.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gpogflqgw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gtramugop.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gisfmmukh.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gzmsvpfal.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gthvheohw.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gsjfufiie.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gsfrhlczs.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gyupaclgo.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/ghzdobsuz.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gzuybghrr.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gnpoksydg.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gjxynuzbq.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/guipnnizo.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxhkpubp.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gdcladkcg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gddzxofyu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvzvzvonk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/guliqfzhj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gpczrwntw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gtyytmunc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/ggrxpnuoe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gvjddvxwf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gmhygnasj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gsptnnkai.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gdppuqtzp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gxqstixfr.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gnwgqcdzz.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/ggoggnpnk.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gobxhhrsy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gbnupyttz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gkkzgohxx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/ggsvymbiu.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gtwjduvrl.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gzhmfygdr.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gymbgyqax.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/govercjxu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gaxvbwnos.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gvkslrpqi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/grdisxvjn.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/glrwvsjkd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gxotowhep.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gkkifdynh.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gugyuhata.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gexepqaaj.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/grhdpyftp.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gljqezuqa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gnquykywp.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gqmfllaia.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gvocgvuxl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/giyfzuiyz.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gwnrfibnm.sHtML


<!-- 参考信息 -->