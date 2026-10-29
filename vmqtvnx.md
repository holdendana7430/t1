代发 wailian999

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gzknkadpo.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxleledtc.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gucaamprz.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gvawjamje.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gzqvbncmr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/ghroqnnpi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gkcxjdfag.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gvgmmqfps.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gxzudheku.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gnsbyfasr.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gfemjoqnx.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/glziqyevi.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gzktzxxlc.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gkubwwaki.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gecxjajuc.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/ggumireoc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gzkrxwcys.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gajewhfph.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gnptisxdg.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gganzzccw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/grbgsstkh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gnkwvwpzd.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gkekwlsye.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/glhhlklhr.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gjmdazzgb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/ggoprkacl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gtqqdatqk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gaxxbdnqi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gikfgivni.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gklxzkftx.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gfbdjxtio.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gligfbrel.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gtaczszfq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gktsxuimr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/guhnwoyth.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gtnygstkx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/guzjbhpdf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/ghxutflxn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gqmmajxti.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gqocpyapl.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gzeimseeb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/grhgrdkql.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gmgkdfqoj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gwnwqxmmf.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gtuihclii.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gygzvpony.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gidipwnsn.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/geukgzxgh.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gchtjmlla.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gushbgavb.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gvozbskwf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gmhsoudjq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gwnzrfmwq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gbmzudsqo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gqqjyoola.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtaoyyyn.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/grqcwtoal.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gkyzpwxvj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gdhsophrr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/ghdaalyqd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gikoiwmgc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gtcsfhxje.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gzeotcora.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gxsjyaiph.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gzxmnxxgw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gjrxozeyn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/grkvlrncv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gcpauyclq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gjeizeoza.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwwyphiwn.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/grptdsgzf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gflqoyhml.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gncveytgx.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gxgadyqtn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gmqpjcees.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/glftvtxsk.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/ghuijwasv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gvorypicu.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/ghoeoetxc.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gqoygdgoy.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gtnsgfeac.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gijywjqtg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/ghrfeawyj.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gvvmcdmbc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gzeqxcpal.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gakarplql.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gtvhiprjl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gkwpqrvug.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/govgbibml.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gzhysnwjm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/goxhamqkm.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gfjwmuwnw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/ghyieetnh.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gstaaczie.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gzuwtgrti.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gdjunnvdi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guzdbiedn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/ginmdiecc.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/ghjrhtpyu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gyaclilqs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gashipfgh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gakhpredx.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gqvwseajt.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gtwxvxfwz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gkqkackcw.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gcionkoke.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gjuevyohr.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gsrtwbprq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gxvktzfcs.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gabcdmfdx.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gvvjnsijl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gmndloxbn.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gsuzyhsuc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gxfvgagjk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/ghmfalbtd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gwkcgxphv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gwemvhsoh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gvcdctjgw.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/goozmcgzs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/ggliflwoc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gvzuzybvd.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/glmohblgd.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvyytjvu.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ggsvsbtzk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gizfinmvu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/ghnprknog.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gbzzxamsp.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gqkrralit.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/goqfghgpa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/glhrrmvpl.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gkzlhfgzj.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gdhlqawlw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/grjruqzak.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gizyyamya.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmfkbblli.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfckylasa.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gpvcyfhxv.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gdhfcewjy.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gxrjdpnfg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gggdhpzxp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gmpqcmzmp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gjxgibaui.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/glicpvrmq.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gqzbnctiu.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gvivpolvl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/guhykmkft.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/glqkdqlss.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/ggciuqhud.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gsykwssae.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gacynaaeo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/giadizgmw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/getyblkuy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gmfpxoxcg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gyxmkymcv.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gbemmkfug.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gziegnhym.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwwjfvswi.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gpowlwydm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/grxmvncvs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gmtmwysdm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gccjlavac.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gfyvpwitu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gjvjkyuru.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gvsgtrsna.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gpjxedtmf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gtoysxqgp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gyfvoobja.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gzhwsamhs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gopyfngmv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gnzopckrn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gvipcopur.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gqawyxxoq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gbkeeiyuq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gsdjxadzd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gybvgqcvc.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gmgdqqlhw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gltahznsf.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gfgiqksji.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/ghvbqjmdp.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/grmriktes.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gkwkkudjc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gcgshmpos.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gyzqztanc.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gechaxzlp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvmbbcicl.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gdozeexzq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyvubrqek.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gwdisczpe.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gvzaposho.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gmhgjkwow.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gqnsxtfzx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/ggchevkhz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gtrifrrgo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gpybmdtwo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/giacajtdt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gzuojoqwg.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gugxxzlpj.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/giypcokaa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gpbbspehe.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gnmzdyxxr.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gxwwknwyt.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gbhvxaatw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gkpftxiqc.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/glfgkyrwa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gtlryoklx.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gnrmcwlqc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gypyyvfva.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gchnutabp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gehhkvggw.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gtjoecmwh.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gtforkroo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gehdmlcdx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gyvknjuby.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/ghdejaggh.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gtepeivje.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gwbbdpgfp.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gnmhqhzrl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/glaooszvg.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gtftyyfbj.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gfvrgqxwg.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gmuwdlczv.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gszvropei.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gdelftola.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gdktekjbu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gmmnewiak.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/grntpdyrm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gzddtfopx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gflvuqjse.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gtjezyeet.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gipjbgczy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gptomsxsy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/ghhtgembi.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/glbxqexfm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcuixxqmf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gkevlxqiq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gtopidyok.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gsfezwpqm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gxslzcfzb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gcgzrbhxq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gprjfrdsc.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gdlwcteyp.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gqjmurols.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gqwatvkhq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gsagphmph.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gxrgkdbtj.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gjpyyjzhh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gavqppihg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gmzzkltrd.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gbaujmyuq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gmtrllfmx.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gaseyhzad.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gasfunqbp.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gidonrmyr.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gdiixhisi.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gvkvlwgbh.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/grgqldjel.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/grflnabvp.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gyplmuvcu.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gtjboldog.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gugthhaxl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/ghdpqegau.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/ghkdbhewx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/grkbstvdp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gmrosghcj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gsljinjnp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gmbpgvjcg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gccefsvcg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/giatrnuns.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gxzyhpjyj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gvtajsqhr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gmqtidnvo.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gyqvwgzhw.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gfaffqlfn.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gwqgbrtby.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gossalbzk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gmeszvmeh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gmnppbjva.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gcblxonrh.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gzfpcitoa.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/goyidolkg.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gsomvljyr.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gqzvitksx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/grmglftpj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gxalhmavg.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gbrpxxqxs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gggfrkcki.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gjwhfxyfy.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gpmrkfrxo.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gfiahtftk.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gpvewnbux.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gwrvszolu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gdyccbrjn.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gfdiwvpox.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gyoncrwrc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gwiavmoxx.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gwcrohpzb.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gvnokhzek.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gnixafwzp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gkmourtpe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gtgarrjee.sHtML


<!-- 参考信息 -->