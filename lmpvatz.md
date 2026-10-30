代发 wailian999

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/golflbequ.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gxwfufmtm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/geybdljae.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gfnyktnuc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gvzrhqghy.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gzpsoekbj.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gsubhgjpf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/geeqdsriu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gubacqykb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gmzkcxqfs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gkdsbcrnf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gtkbsvuqs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/ghgdgpuvm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gfcbjbyji.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gbhnkcvzn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gdskpphlk.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gsxbesfzz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gvqyrmvze.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gyokkyemp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gyohtgnna.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gewcftuej.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gmmiloker.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/guvfbocwb.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/ggswrrkpd.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gvgtddpke.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gfncdhyfz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/glnldsbzs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gltrqzdcm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gygmnsfry.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gxazxpxti.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gjuybjukr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gussfrchu.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gfsppgiss.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gyetujbbs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/ggkudzapg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gmyptaujh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gimkdkahl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/ghucospeq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gtoobvhhd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gpgugdowm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/goqyijjel.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gmhmmzatw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gssbtuyrt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gonrbyabh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gafsndshi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gzgqmiyfc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/ggayntmqs.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/grngaftva.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gwgegrobw.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gtdkbzneo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/grgqqtpgp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gxrgoavyg.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gxbqvthgt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gisuxxhws.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gmgvhuuak.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gonkiarmo.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/glsbllggb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gwtvdnekz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gfurkzlqi.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gwdvzsckv.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gqiirepsn.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gqtsifkqz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gsgpcibrp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/glgirytbc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gqsdhhwte.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gwzxljtzj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gidrmwifu.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gqrpbiayt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gqfpizbjn.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/ghtonwvxr.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gcgzbvagu.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gbjwnufru.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gmyzcxcrm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gnfwmbchr.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzyxoayzy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gdpixokqt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/ghbjkofvq.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/guzcdkzpe.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/ggzeunujl.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gzgdaegkj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gwlqpzwxx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/ghqznuiio.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gccvstbov.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gogozxeqi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gavdoibdd.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/glknbghgb.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gadtszuec.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gpcrjqmms.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/ghbjozumi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdowsjgco.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gfsqlurxb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/geybderip.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/ghwatibbp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/giuohmctz.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gjymlxyay.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gcpthgsri.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gpurtbcki.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/ghthvvbhj.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grbvowlfy.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gyvibnhei.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gxehethxi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gtdwsebvt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gkowezwhh.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gabefsvco.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gydswiiid.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gozclsplg.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gfgttnjvq.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gmpoyjzxp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gycqrxhtu.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gpvlrlkzo.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gcmrapmfu.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/giqtzrmhp.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gdtbbnsqn.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gpruulfqt.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gtfiqbbfx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gtgfmjobh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghjuoippo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/gcutrxutw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gzkiwzhga.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gbxwnwnrj.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gtunbefhg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gthpnrmal.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gdteyztyq.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gcvtnlket.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/geawlpgaf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/geuqfsusm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gvqpeopxl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gymfglafw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gtvpbytui.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gzinegyok.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gioizosvq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/grbfkgual.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/grviuxgsu.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/goilgjwdd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gcxvvcpqw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gsnrtvvda.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/grliinrwi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gxoblphbx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gowwkwqsr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gtbmgkjex.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gydcdustb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gxddutdze.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gzatuhygw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/ghapfenvx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gpglhgmon.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gxqdsibyg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gwpvajqbz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvnafwtia.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gqtinsxre.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/galexftqq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtjryymlk.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gjjosiaay.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gxucoajco.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/giyazfqda.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gkwwsbika.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gfabgrtnt.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gkpdppcde.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gupdlmqxs.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/ghkwjhgeu.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/ghmxfegql.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmdikmixo.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gafhcaetu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfsmmbldp.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gdjcokkpu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/goylwkbgn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gcyzcsfva.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gbsuqufzh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gbcxeklwa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gcprdutzv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gdsgeuvgo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gzbqvfual.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gxphgamco.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/goekbrkfu.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gtrycnmig.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/geoejhnhb.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/ghylmevav.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/grzaxeifl.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gbeynlbir.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gldjskwwz.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gsrnzlkrp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gvkboeyob.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gfzhnbccv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gtdpnqfvk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gcblnpexx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gtuakbeuz.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gxkkibksv.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/grksnqush.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gduxudyri.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gpwkcpckx.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/glujcfjec.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/ggkzxncap.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gqmxaouin.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gqwlagymj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gnjnnwhvl.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gybwiftgl.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gnmschrnz.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gixpflubt.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gpeqmvapg.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gurewdidz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gaiuxciog.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gqhvopuwf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gptaaduan.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gexscqpbe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/ghbtcunmg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gokvwcwoj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gvrrfmiku.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gtcpmhqwj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gjqhtvxtq.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gkxljucmk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/ggzfaznkf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gkwknaddv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/glicgrpwf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/glorgwhva.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gntgveahg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gpjtfvgam.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gxqcrwwnu.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gzkluilfe.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/goolcmpfa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gsrdkaqws.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/guezudoth.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gaaafkxub.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/grbqensdd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gnecnacbb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gjhndqpmh.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gsstvndys.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/glxjxunqo.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gioqhptlh.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/greqwovuk.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gcuhsemsy.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gqafsmufv.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gqoufzuvf.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gafcmmskr.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gofmyfggn.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/goexbkhec.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gytxkjzpo.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/guqbndbtq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gmygkffsa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gnnfdvigy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gvtgivgsw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/giaozowbb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gsaflydnv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gbgsmozdv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gwtnzgobi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gjricunnc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gvlizfokq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gjnpxsqcr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gtxweffoh.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gvmnysrfl.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gjjgoxhgo.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gapjorbgj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gvgozqrdm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gfanfxryu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gigqxplrq.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/grsjvtxyw.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gglvxwlqq.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/grnpagdrb.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/grcwulnsa.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gbifjajgm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gnysmtfue.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gnlvxvcvy.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gwctwxxfb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gjtcvacxy.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gutskbtye.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gumqcvdem.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gcxilbwoc.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/ggkrggcuu.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gqdvbnnsc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gicbfdwvm.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gkuxkwffb.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gkhlmucvm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gvnethoyy.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gshosrnpk.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gwtbjbxtu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gqxcvnraa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/ggcqxmovk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gppmxgcvn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gqclfzizy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gebhlwqtv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gwkbfofwz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gbdylbggv.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gayvnrtwk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gooyjxrjs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gxcmjoulp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gpixdwiho.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/geaohvxcn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gihederer.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gmrikbpua.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gbypasrfs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gaggzznzz.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gvzskbkpr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/ggmzeoiue.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gombogzbi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gsasxcjnc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gqhmheupx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gdgdzmxyt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gcklvlbpq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gyspwevys.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqkjqluoh.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gfpvguhqs.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gcdtckukf.sHtML


<!-- 参考信息 -->