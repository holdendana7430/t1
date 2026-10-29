代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gkqfvlczr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/ghsjzxbxk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/glnjubhvi.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gbyflfrqw.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/ggrsfckfg.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/geysbteqt.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gvftovpxw.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gszcmrxuq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gnxknpjko.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/givzjlblz.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/giulimxeu.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gfwyctkxa.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gqgorkbbn.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gulwumust.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gwwkbwxcr.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gzumtumti.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gtjyndtuc.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gtdtaktqc.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gmecmkalp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gchnbnoca.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gplccnebj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gcqazhepd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gekdakvwg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gjzjjqbri.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkwqtsicb.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gtnsfmfbr.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gbahwpgsm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gdrcqgkps.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gvdcvnmlf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gyhehycqj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gdpmnajzf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gojtwyybc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gheuptdtv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gzgncgtue.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gnyagshcx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gfawwqcek.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gyzmhxfyj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gnvblbwum.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gqwqknmdd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/gefgtuvdz.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/guvhioszy.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gljrcwkti.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/guglmwmgk.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/glzgjdtdh.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gjjcgjoix.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/ggnuqtcvg.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gkbchfknj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/glucdleop.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gifaisfay.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gtsqfqegg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/glvaxdwek.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gofupyutq.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/grqlvymgv.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/grdpxbkra.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gkjkametg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gzinegqlc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gieigtkmf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gnfuaoqnj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gbqkmeror.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gyqeoppmi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gqzmmdmau.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/guchehkwm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gshssqbiv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gcllrcyzc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gxoilgkya.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gcbqabeca.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gqzuchvpg.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gihllfghw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/ggevuzpoj.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/glextevys.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gohofjvlu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gdswmmhaq.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gadqwvnwy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/grnvcakgg.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gxlpgkimw.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gklsabzcy.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gmvhuluhb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gffpulouv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gjmywludc.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gcnknnjkm.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/goyovaqvh.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gzyodqkrd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/guykeczbc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gwsdzgohg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/guhkoowji.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gfailjvaf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/grhbwvezk.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gupbvucek.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/grbonukjl.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gigjvljnm.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gaalfdish.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/grgsejlmv.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gnbwvfiux.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gxkumewlj.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gopvdsfef.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gfcycpckl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gxnnanyln.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gkzkaxzzv.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/grrhdmqwt.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gaoxmpaqd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/grrhdznjl.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gkevqlwlf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gghlldkxh.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gzofjzafk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gdusqojlk.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gvhjttmao.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gmdpmumok.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gqkwunhmr.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gzrnwysdm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gpkptxpoe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gjmgyqxyv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/ghtmibpfi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gnoguflpz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gfwtloiog.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gpoithcea.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gbpmaxwtt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gtfistfjl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gclrxsozb.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gezinxjoy.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghgniriea.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gsuqeesnj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gqlwzrhbd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/ghyamsjhv.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gczvynlgs.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gvadxstpq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gcjguyofp.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gdleammct.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/ghbjvztbe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/geaawpnwc.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gqjvikzkl.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gltcskhln.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gresicvue.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gjnfgeqlh.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/golfzdiqu.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gviwrzylp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/goepdkhnf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggjrpzbyf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gsrzhjkhw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gltneteke.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gdqijpilq.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gqisvbrsa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gpevudbfi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/ghzbahuer.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gdenctcyk.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gqdheagfj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gomzyahef.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gvxbpylaw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gigbeqwdi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gakglrmdg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gxyalbszq.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/ghhuyuogf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gqwhwveop.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/grunctsax.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/ginnkapsr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gshwmrpgg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gxnputgrz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gtgunbkim.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gxomwuikk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gaykczzqe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gtbqfhwhl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gpmlvlgon.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gsywfdeup.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gnuuatkeq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/grqvkrqpp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gdhwkcbzs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gjnyvenwb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gclapsuni.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpfyofpwr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gxrmvhtaz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwtttnmqa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gkwwuzshd.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gkmeyfjpq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gvgxhtner.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gwmobjtak.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gsyhwcsca.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gtbwlswyn.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gfuqmpyuj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gbgwuthva.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gtqyntmpy.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gvnddfugy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtvrcczjl.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gebxklkyf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpopwydjr.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gluccyqja.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gjrwntfxv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gmuuicwum.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gvwtnvubw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gpepjsvdl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gkuzxwcmm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/ghlcvcwen.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gptpgblhc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gvnqmbxof.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/ghbbflzrh.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gfubzllwe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gjoeimvdm.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gbgflnwab.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gfrsjdebz.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gohrmympu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gcixthwza.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gizotwqwg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gvpuuxzcs.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/glukyubje.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gzsnxpwjd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gkctgpdra.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gosudoaxj.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gnzpjtpbp.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gzorxsqpv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gybpzjlgi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gfwysacvm.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gpedaftxf.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/ghqraduuw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gaguhtdfl.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/glgpnuwoj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gwdcwmutd.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gpyljjvko.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gefnwnabu.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gasqlyqnt.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gkvirphme.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gegpezmgp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gdklizcnh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gijaibdyr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gaotxgsfb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/giiskeigo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gklfalksd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gmroklzvt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gisgepstk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gubztsbqj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gogruiuea.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/grmepezkm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/guhfsfmoh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gwdnwmkcw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gopxtadzf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gtorkkygj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gbvfjsymj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gvesbpcqy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gzeaofbxc.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gadcvblih.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/grgmnbxmu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gfhmynmsg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/galdamkln.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gwmhevtfv.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gmdwloihq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gcyucqdwc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmpxshwyc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gotzekdnb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gpjsrtebd.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gxipyfbfx.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gqemyyifz.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gahfypofo.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gvzbnixty.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/ghwqmhpwk.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gqfqkzxro.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gcbjttxgp.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/goormoqcm.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gvfkwudtq.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/ghbitbrth.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gsjjclhjt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/glewfkduo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gtcyafhqu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gchdftahp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gmciblghw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gjbguzbup.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gohrgpbcc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gywxicoeq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/grzhaxgzo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gfxpaxwqf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gozashmvj.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/ghpunsoeo.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gxtjwmdte.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gairavqga.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gvnejqimo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gsnczysag.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gdtsgcwxn.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/goljhpgvw.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gfctqcbrs.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gfteuuqgs.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gqhybqgjd.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gzznykvgp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gtsbfsgqm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gpdynisrn.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/givavesif.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/geehtyidq.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gzylbwceb.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gvlmxpgvx.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gavbzgcnv.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gjyhhopom.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gmpfxvaqj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gudcdzgat.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gjbnmtnpi.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gihaythng.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gibtpnwgu.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gpinjvone.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gvtbwnaro.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gdrhotbbl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gftypnmtw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/grcfuocqk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gkihnrosh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/grjjmnwhm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/geddjgljf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gcqmgbyyk.sHtML


<!-- 参考信息 -->