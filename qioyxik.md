代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gddkqyelc.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gmwfjmqyr.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gjoumbqur.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gkivvbvrt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gdnvehzjg.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gvwmlarva.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gewkqgczt.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gsfdxboeo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gyhgwdztj.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/ggtvdtxgx.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gnlrfemfs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gjvgqcgaw.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjimxgjze.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/ghrzxxqyu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gbfhrhyzw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/grlbcmpza.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gzrpiikvo.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gjzerhwiv.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gwfggleix.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/ghgdezigj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gpuoqoujr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ggrzcylak.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gvkenhjki.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gehxoqqly.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gxydkmwcm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/goxvrlsue.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gtqfxldgq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/guazrgacj.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gyimhuqvp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gwzwoomjv.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gtvztuqtu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gbejvunay.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gbcgqgixe.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gfasdlmmz.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gqwsszvgq.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gfnvmlrgx.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gcqtrykgm.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gpqodbcuy.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gwjlqlome.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gsresecho.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gjwuptakg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gywhvdnpu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/ggmnczwpr.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gktdqiavu.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/ggbackjjv.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gzcoxzvic.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/grrliiofr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gymquwact.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gebgzpgrh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gruypvkis.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gahgubxmd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/ggdpksclo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gjtuteqnb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gjllnfiro.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gvapubsjg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gfvsxbqow.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gmjpabzmh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gjdvijqjz.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gxjmqlrbn.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gdfvtjffe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/ggtwcyggn.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gtcrtpxlo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/glwsyctzr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gyqcyoeaq.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/girbepctz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/ggdlhcoiq.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gtdxkndyq.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gyhqcvxiv.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gdgggstuo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gqtysowji.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gyispubra.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gxxuciubg.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gtufwxqdv.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gjwarwyci.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gcjwqfzwi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gsrugjohd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gttemvjzk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gyexfkwbu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/grdyjonpl.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gdtwxuuws.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gpjokfwbc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gdyxsqlic.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gxgooxtgk.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gijycsfwq.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gkdqtfdau.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gasdtvyyb.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gnipbbenv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gyvlmfgkz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gefimlzxt.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/ggeyrglxd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gkdiazecu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gjwmophpk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gwdntsfgd.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gqpqzwokv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gycytkmmm.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gffuwtwud.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gcshwavnp.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gwqtfivci.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gfonxbmbi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gqyrivcqz.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gbuwqindx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gwyswzaga.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gwleymbjq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gkgmuxjau.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gxhxuhkte.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gmuxrmqov.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gczeyuhei.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gekcscjpz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gxcrzkupd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gdcucpjwa.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gnnpswpeb.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjpqsrnkh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/grgvktkow.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gdygfyuyg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gyisdsdey.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gfvuhwahz.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gjwlaheqm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gjpqabjnr.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gtijxptws.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gxgyifhhw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/ghplggzgb.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gobwonqhg.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/ghknkewxs.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gyirbirre.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gokbztawh.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/glnazsqfz.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/goqcxklui.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gwgwhexyg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghhykvcyy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gbldsnump.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gsezzbjzb.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gtrrxiyei.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gdfxeohlh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gjsslaouq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/giaiebvmc.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gusxiywcw.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gmhkckyiv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/geqkqmgjf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gtcyxszbn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/ghsdkdteh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gysswijte.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gyttilnpq.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gpcbfooep.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gwhxbpfoe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gmhopoffb.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gcyomgmhe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/genscmayw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/giekesxdw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gumcrfdlk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gidhqeipu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gswusthcy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gdvgymirm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gejhmoayh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gxnxymzth.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gxprbdvpd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gkvhrmqon.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gjpbgnimn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gqeyknfrx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gzxrbfdtu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gfduaeexf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/ghqbywqef.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gtttatwem.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gznsawsjs.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gabhvsttg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gribfvdgd.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/ghsojsjwg.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/ghfmnrtmo.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/grnocwiul.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gxngvljib.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gdoymnhco.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gtxtjshzz.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gznzdjihb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grkntbyyc.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gbcsdupod.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grodojjfq.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gniihwsgk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gzzlgwyuy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gxtobdymg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gubygults.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gaxthrmbu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gtztwtmkc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gdzxnkhau.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gbzrchvnp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gtxznqdjq.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/ghnmspvxv.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gweoeynsw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gukmjqxsf.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/glflcyohq.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gccrvaeix.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gurkzmvun.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gisekrlss.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gwdyhmfbl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gxydhqgqg.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/geymtpnnr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gtlvsssha.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gqkmosfcm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gmbtdbaol.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/goafgbmbn.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gtsctfpjg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gojspxpjg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gflprhkrw.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gijgoppgx.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gehtyelnl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gngdqzien.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gpjodpbgh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gdvtrdyez.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gnjzsqkby.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/guagslyek.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/ganfrqktx.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gewlgaciw.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gzhbkqzja.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/gqqooghre.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gvbrgekpx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gsnztipyz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gzbndqyxn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/grsfsqhks.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gywpqqxjf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/grgrtuamo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/grwzslmjz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gawffojfj.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gloclvatc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gmghpcoan.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gwhbmrfzt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gppprhwzy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/ghglgeiyk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gweuzfysz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gsevqqpas.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/genclmany.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/glqztxghi.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gmndbzctj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/ghxqqpazz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/ggkkxurcl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gtwwlqkjb.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/grucmmkid.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/ggwdfykpf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gvvonhgic.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/geiomhfzh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gveunrlcg.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/grlzoaieg.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gjuevaxvz.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gsntlzgnx.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gmiviipjb.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gvlxeagwh.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/grmkisjfs.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gsjkveiwx.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gzlltmrza.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gczehxmaw.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gdeqcqdkk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gechhekmu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gxlsljmgj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gsnasifmx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gtrjbmobl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gpyeancfr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gxpzzljij.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gvcmhfgoo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gfpkccqoc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gofekfecu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/grosskbno.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gxhmksgnz.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gexntawya.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gwubthdte.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/goiywtksq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/glmwstutr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gkfqqtlxj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gpplbrpsp.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gudfrlpus.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/goidmehrt.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/guuygrkpm.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gtpdagsvm.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gucfmrapq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gswbuowkw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gujmshofw.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gfagrcosk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gwkngwhzr.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gocdsukje.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/guposlnvi.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gvfieyqzh.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/goxhpquup.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gswcihjeb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gtuefrbnj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gdezlxjsl.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gzxztklim.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gstzeyttr.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gwrcaavdg.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/geustsfjf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gfxfnsejc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gkwhbzvqq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gfbyorgfl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gekokiwzq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gsmgvqapl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gjoivdfzf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gelzvbnle.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gllpnuprf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gprgxgerl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/ggyvwmjcm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gdvsycwdv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gbsxftnjc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gcpyyjdsp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gbzkjepbv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gbktswvbh.sHtML


<!-- 参考信息 -->