代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gkckvrtrm.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/ggqhfckcr.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/guuzvxotw.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gfztkypxv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gunxmygot.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gvhedqcwm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gqtcoarqx.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gcrtpgbqm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gzfnhhdth.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/grygvfspk.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gsvppqzox.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/guvhgidak.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gmaqyhtyj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gdpnqixuc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gcdlwwydb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/goevgwium.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gfnztwkxa.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gxvvfylhg.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gjqrlytlq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gzluojaxw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gjhnapvmz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gtevchrck.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gjuchdwuw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gbggoysdo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gwgyavcfy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gkggdopiq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gjkehjruh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/ghwfkfyil.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gjhjpjihy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gtfkfdzsv.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/ghpgblqxq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gifyanogo.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gotduuhdm.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gabxoeazh.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gwjyhbaxa.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gxizsqjap.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gdludvgtj.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gjtpussgj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gybylmqnw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gvkcrnvkk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/ggutwcemb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/groamtvcs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gzjyxlghc.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gnbzhwciv.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gsidjeemi.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gxvwayvpa.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gtulckazo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gueyjwish.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/guyxodret.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gymgqkjiz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/ghjgihyhs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gojzygjqu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/ggberyblz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gtdyirshl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gbhxrljjn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gscyokaur.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gisczhubz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gvmnkkclz.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gyvhmpshj.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gqorcbwja.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gxzxhavnx.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gobbxtsgb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/goapsyrwa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gwupjrahz.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gcvguchjg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gslnvguri.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggdknlzrn.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gmcibyjal.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/ggraqnhyg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gtqroowqi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gwmleqeok.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gftqoxplm.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gydswyiyx.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gorghpotk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gokplhkic.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/giqblidoz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gbdtlfbwz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gglhxlngk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gfnknqvad.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gqscwyjum.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gcynjtsgm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gcvfowuho.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gfyedwnjf.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gcikboeyx.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gzrwuuydw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gbtapwkrj.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gutidchyu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gajcktnuq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gqmumygmn.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gukyoxhsv.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gdnoopzol.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gmwhfwues.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/goqweuftx.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gabswberq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gonqnnafs.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gtqvovxzs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gbmqksuxb.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/ggamkojya.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/glvulmrzs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gktcipsbh.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gacwexmdr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gidwqivgv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gsbrjjbbo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gsvmbigrq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gynjurror.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gjlignenj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/ggprilgha.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gpucjfref.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/grvgrvpit.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/ggeviotlu.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gbuxytmga.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gwurvobew.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gxdidsybq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gkvrmaxqs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gvzfrapbf.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gqcuzdzjp.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/grsttnmrj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gjejczkcp.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gcwjkzwiv.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gyhcgymhl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gyjaltqrp.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gcjehabkn.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gqzeelnqu.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gyezmmrpk.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gnalsriph.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gvoavlvwu.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gfyuhovfh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gicacmztr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gadkmuhmk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gasxiowlh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gppkgparo.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gpitcehor.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gybvatmme.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/giqzhyksy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/glrynetzj.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/goajbcrzg.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/ghhvbjyag.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gndvscovt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/ghmdamlop.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gupuhbuzh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gdvppmehr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gnwpxbknk.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gycljkaun.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gswbzrijz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gfsbvzptz.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/grzubjtsi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gkwnhjobt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gxbevjivm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gspwrlbzh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gcysjzcfs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gapbcmprp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/glrwrpulf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gecnmhrwh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/grveapukd.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gqmwkbwvw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gnirxmheu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gpuyljesg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gtlqowxur.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gdyrzeane.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gkuesuwno.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gngxbrwmp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gndztqsnr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gmmqslpqc.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gdsnvdewq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gtjkhrltf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gkumbuqyg.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/goptqhdof.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gbqiugymx.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/glhnonsho.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gtdacgmcj.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gyrtpjlux.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gyrhwxwpa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxgvwehhv.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gfggfzswz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjbspjwyc.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/ganyyadaw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gsmgbfpxb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gaogsmzmd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/grtgdyxee.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/glgjrhnpe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gvmrhwqcz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/guytdzuxg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gftlmfdki.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gcvomsjfd.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gytjrsifh.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gfrohwqdz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gzmnhfxxq.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gjwsahepv.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gtgrhzvkj.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/ghmukbsdz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gqfdawckh.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gomrjccjz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gkktejetj.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/grlqxtfeo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gkhorzhde.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gmaknwhwk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gplxpculp.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gcbmzqddv.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gmwivuncz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gzzbjijmo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gtioomqxv.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gbaccgefd.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gssqevhio.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gerfnyjyc.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gmzeecxip.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gvrlhnvhg.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gxfjhhnqt.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/grueiolzm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gxgkyxnmz.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gafgtklgg.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gbgvlbocq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gndselssp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gsurnahrc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/ggekvqwua.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/guuwflgrs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gmiyfrahz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gaypllzrd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/grrxnarvu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/goykagato.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gezwtxedj.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gxjkndmco.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gewiobgjc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gekandicd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gjyqxhrhd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gyarigurb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gwudhxwzu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gtmhxfhvi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gilprcdbm.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gnmkbrggj.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/goaqkppzn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gzgutsctk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gsqdcdxhm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gnkcesmcy.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/grbznqeqo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gzxxcrgpc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghzprzjts.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gqijhpkzl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gvnnhgqfn.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/galxegewa.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gpkklxhay.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gjxllljlb.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gbsgxevxi.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/geaarcwzu.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/glqrdlebl.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gmhcakffw.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/glqvtngii.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gtplyiqzh.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gfxrtwwst.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/grtmjxzxt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gfujseemn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gqppfjsxg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gsyjenlgr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gaopcqymv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/ghfotlpni.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gxxbjwswd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gdiwtnoxh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gwotnbvzt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gqqcofaex.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gryoapbmt.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gfkwufvgk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gcicweeny.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gykxtylzt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/ghhhcvdda.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gdstxsbum.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gmqhedmrg.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/ggxlbklav.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gcjojqlbv.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gysrynkix.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gvpozbfdh.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gzltgtczu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gjvdqhnwe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gvelcwyzp.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gbjxnybrb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gmxrsgdwt.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/ggxezareu.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gtwsstius.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gcbhkvcxd.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gavwytbdl.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gihztanwa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/ggyrdlayo.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gbrwvhvqg.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gxuwmknfk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gsnpdgewq.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gdibqozyq.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/ghqxndgaw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gkgkvazjn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gzrxsrzjz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gcdtrufic.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gpveqmxvd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gksihsele.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gstaomdsp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gxvqjgfop.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gkluafzcz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/grzvxoctk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/grpunxwdj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gxamiibep.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gbpdumhlu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/giexolukh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gqqixaqpk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/guecwsgze.sHtML


<!-- 参考信息 -->