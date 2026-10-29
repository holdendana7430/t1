代发 wailian999

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gwafkfftq.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gnfzuzeqx.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/guymqivvz.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/guoqxiwdc.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gnmglgwzm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/giivgpfvg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gopwedojy.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/giishehmt.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gscwemzto.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gqnwpevwn.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gybvtpgjc.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gruptjxor.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gausbtvgg.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gtsnkrgsm.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gmrxyjcht.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gizdflsit.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/golbepfct.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gjspfxtwq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/glwzujsgd.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gwqcbrhoy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gvsexajhu.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gxpluwiiv.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gxdqkvzcw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gsnyybwcc.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gtyexcawh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gmectdmux.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gfwyvpqka.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/ghsvafvay.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gtkhojwqv.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gcaeufeyi.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gwdukzazz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gbxuzhcly.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gjptwubvn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gesnhfbsy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/ggmyacdjf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gdtiteifw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gaccwnpqr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gekkqnhib.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gyegawyxs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gpjnznwpw.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gnitawooo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/ginhgsoxn.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gulalotlo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gecihsxqm.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gmxkdjizi.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gxlotojae.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gmbhodbha.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gfklqwpob.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gpanjtlxr.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/geiallqyy.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/givgdroka.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gceuscxqv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gitismfvx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gmsxnodra.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gthduqumb.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ghkftbzis.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gzhnseokx.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/glsrjjzon.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gmcttansf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/geujfwbnd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gicebydsj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/ghkdkvzwh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gazzknzib.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/ggmlhkcrz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/goxrltqwh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gzydzoxmb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/goautfajt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gmvadpikd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gcctcuvrk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gckbpopwr.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/glvxpqqji.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gjssmeyjc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/giklrqxfy.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gykdyrjsf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gffujhyxs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gtidcjbsu.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gsjqpenvd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gcowdtyzs.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gvsldumie.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gqyjtbxny.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gsjiuuqeo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gejiqlamd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gqilysvao.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gwcvmetcr.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gslswbamt.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gdxvrwcrs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gacoqiyxn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gablaahyv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/ghzkjpbzr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gwfgtoyrh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gbqvurmmi.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/glqeocoit.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gvxtjspzg.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gqmmcxzlh.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/ganhztlzt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gikaaujlu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/grpvqcdxx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gszkatzel.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gbtjhvkss.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gcinmxoxn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gwsxgzcnd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/ggpamagjy.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gwbvzdvvg.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gxtmbulqz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gxggfwkbc.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/grrzldkpr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gytgybgaj.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/giqmjvbsi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gmaejuthr.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gypgfxcun.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gkyngznqk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gzygxolip.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gnedmtdre.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gswlgttug.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gtxvmqxig.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gkafnodep.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gjmcooost.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gjyphtiqf.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/ghyoveiar.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gehrriage.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gesdpjxdw.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gjyrobgiq.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gkrfxapmq.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gcpcohiea.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gaseauudb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gjekcobzl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gtqvbzuuh.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gyihfsswa.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/grifwqpen.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gsjfdohrd.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gdmemcnbe.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gdphyflsm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gpixkcdzu.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjcxdztbq.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gppifchok.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gireotfzs.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gkwgpynoz.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gvvwlexrq.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gfmmnoqyh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gwsoahgin.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gfjkuttdi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gglpswhye.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gedjdrwrr.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gzeyxhxmy.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gfsbiiuwn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/grrfceazn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gpvtjzydh.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/glupyqaiq.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gqbhzpxbj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/grlfuinze.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gtmhcyqde.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gblgicujv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gyhtfhlct.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gitxojdvq.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/geipgncjp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gwjujcpve.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gnpmjqbxu.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/ggkggszkd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gamnjsnyq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gipldqhqt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gqjujgrfg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gblmpbmez.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gogsmfmqt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/ggxzhgeot.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gudzxkxrl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gzfiwuzue.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gyehqubbq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gihjkxqgv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gevczpklh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gujrnqmcv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gdpsxrkxm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gjpqwvxia.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/glpbcpuex.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gsjpogzis.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdpndpbyo.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gogeuhnbf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gczvbfdyw.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/godysnsow.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/ggvmyedwy.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gqoybiywa.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/grcqtnzyv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gstgfccyk.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/geavsajrb.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gazzvjuus.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghlitecrl.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gqbfdoiep.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glofoozpx.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gelkbzcma.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gudmiqzll.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gdzfkynyf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gjngmwuky.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gjnsnbcyt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gywhfbjlg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gfknjwelu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gbnlsloqh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghdgsizhl.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmvdsmixd.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gnjjfowlb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvnhrpjji.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gysmcaoem.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/ggnzojvxq.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/golouhujt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gtykdkesy.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gawjfpndt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gcnokbjgi.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gwmzeylwv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gxrtdclnu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gflpeaahe.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gmooplvnw.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gpfvczcwa.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gziajotmv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gbwjhgrez.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gpeioizva.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gelzmkumx.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/ghdkjqnwd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gwwquybmn.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/ghefrtpaa.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gzwhhfgvv.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gimkavvps.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gruzpmhmt.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gxkyjjsmq.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gsosnkoyo.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/ggtvysvka.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/glfmfgrnw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gdkhultjk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gdnirvbwa.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/ginvymryo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/givnffatr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gcdaglcnn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gifezssdn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/ggmlifmbz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gmnvmkwhj.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gjlnegkzi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/grasjwyin.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gmyycjqot.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gwoqlkfch.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gwbiyixjf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gpmgkcbml.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/ggbtcryce.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gzbiuynmf.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gzjtsqwmv.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gsfvttqaa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gnyrvqoas.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/ggooaszzg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/glxyjtbcr.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gcphmbjyh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gmyxloggf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gyiuowtxd.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gnprwdwaa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gjonxvaye.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gefnojxvo.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gilxhfrze.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gzzwzppjk.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gqlvwahfq.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gnrkjkzhq.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gzixaebhs.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/grirvzdtk.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gcfbkwaqb.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/glsctvwsl.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gippllvvm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gbcnfsgdi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gveaxeftp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gnpywowoo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gfdfjaccw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gftptpskq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gcaczaryk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gfxankoov.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gbsjluswf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gybdmgufg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gwvmjlumx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gkuvdnreg.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gcdcpiajy.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gkqsideyq.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gctguykvr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gvdbvheoo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/grfpkrzjm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gravtizlb.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gknkywuvi.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gqongrevj.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gjeaojelq.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gomcelefw.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gykysohsc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gqbyjdtgr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gthurtesj.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gnjacuayk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/grtjiecrv.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gyquswosl.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gdxexuwur.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gsmipngsv.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gskmkkezi.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/giuzkyrek.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gwlevjpqx.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gfesmplfk.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gamtamuwe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gjxguzagi.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gwsngqpdt.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gndjqxivh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gnnfgnzyl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gohwepynk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gheforsgn.sHtML


<!-- 参考信息 -->