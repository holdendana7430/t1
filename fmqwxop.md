代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gvosweevq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gdhioycbm.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gpaqrxowo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/ggrjybhuq.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gecxgjqot.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gvlxybnmq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gvwtudvqw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gopryrqir.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gzclxhbrb.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gjlnflahy.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gfdygmphj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gnbkxzaxd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gashwbitb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gimvhwnpu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gexlnikfo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/goijhedma.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/glzeizzte.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gavienulb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gutxtvuhy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gpfbfwwhf.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gikvtfngm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gkaxcxcdr.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gxpfmjctv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gdnlboris.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gekosyodf.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gzkwhvfce.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gdvljulhh.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gvqgjniop.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gbihwvyzi.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/grskkrywm.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gseuxgnff.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gebigubrq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gxxonfbpi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gjdskxxzr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gjaygxipl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/ggbwumddt.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/grbgexalz.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/glklrnvcp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gohbvgger.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/ghbxqxvhd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gezbyjqti.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gngheqory.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gkkucweci.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gtcecoxkb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gucioivoq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/ghzttgqss.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gkjjikbfo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gqldufdjf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gkssxvatd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gptzkbodx.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gbadjcdtp.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/garhkkwgi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gbwiitreu.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gdfiskcsx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gbgkwnohr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gkxgxsbwi.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gyjcfeujd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gtoetsytr.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gsqtkaobt.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gkbjdljip.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gweifljdk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gyfacttnn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gjjbekiuw.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gagpdphka.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gfsyakgnp.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gllsvpgfp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gudgitzfm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gdqtqlrwd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gzoubmafj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gxgalsfjn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gbpiqbzhu.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/giyluknux.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gywfowluh.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/godiziqmg.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gzmccnftv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gbjvbzzzi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ggyiiiwqo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gqimhjlgq.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gggcfknyh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gjakeunez.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gkxqzbvzf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gkvzhdalk.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/glipcytsa.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/ghveeelke.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gnzqjwafs.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gpgejowon.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/ggnadaxpr.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gmzqmcoll.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gowbndevt.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gpuqbroqd.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gpfnhfiwd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/guufagoef.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gxyyvhqhl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gisodxesf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gvrfprrnc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/ghcxqozga.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/giyzvmfyr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gqeofrrow.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gypmkmzth.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/golubnlax.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gdiapqyua.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/grvsntwtk.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gzkooxefx.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gybgpdrtn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gypmqtlql.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/ggjicmcuu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gvqxrpuvz.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/giueawyaf.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gxoetjsua.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gtzvezbsw.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/guvjwhopj.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gmwtxqlqs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gnfxjetvl.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gdyjyhfym.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gmjsgggoe.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gapezzxrf.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gfxleyljg.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/geusiuyth.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gasxsbodn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/ggongofii.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gozaujlrs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gmkpzbddl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gbxjqombe.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gmuydjshy.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gccgizoed.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gjziyecks.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gaagzkdco.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gqzeokqup.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gnkcoisjr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gjmvovzzv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gsblorfjt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gbtquyfka.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/glvmlhffv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gauzrfsgs.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/ghdwmhqsx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/glpzzzwdz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gqvqpmaxg.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gdkgqyclm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/gimkzstpp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gnogmsjyw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gcdqrrlme.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/ghfflxljh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gjjsyvzzm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gfylzcwdp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gaygikveb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/grrcfsmyt.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gzamnikyj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gikclvmoq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gnowcpmqp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gyuahapsx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gplrjohfu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gjkcjvsdr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gbhhtvpgx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfeopuzda.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gcraxgzkw.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmkxbaoid.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gwflgvyvg.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gekgsmsjm.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gvyjhsdai.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gumfjxpan.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/glnhpqgdz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gcfdgzhkn.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gvfdurday.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gqfnivbgf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjjmurrsv.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gmlnmyede.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggfanwetc.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gfnmfqili.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/grrchxovl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/ghbtdwaet.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gnyqxayyq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gglqatsfm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gjwghpvex.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/ghoqfclsq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gabttlooo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/goktxurgb.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gyntkhhbq.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gvennrvpv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/geqmlvivh.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gsbboubgy.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gbpvvvywn.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gdbkvfaya.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gdtryring.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gnclyemxg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gnlatxmgj.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gkkyjjebg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gmqtpntqn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gowusulpu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gbgwafyvq.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gbhkzmnkg.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/geekzgnpz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/ghmmtplov.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gyecisusk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gjxzvtpuz.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gtexcxzva.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gqnndbuml.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gihiulqds.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gijuzjdfc.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gfxvrrary.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gtgbaqikj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gaiijzidc.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gjfrkvkuk.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gauwcrwnz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gygxkjmqo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gthwivydo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gpqbvofgu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gwcvsigzi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gxgxzxxiu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gaawflizq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/guosxoirx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/ggroghdzh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gypcrtqdl.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gaiohccdd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/ghapddqan.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gdmdiojdm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gpqlygojn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gezxkiofk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/grpfntffa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gemebnavn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gqvikokkt.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gykdtabka.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gpdawhtrr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/grqvaklwn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gfqzyihhp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/ghamioilo.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gxhgtrhuo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gerusjsfc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gfiqmcfqa.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gkoxymwzp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gfouymrzr.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gmqbihsfq.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gjddeiuei.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gvbcfcxzu.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gdghdmjnz.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gevkkqzlu.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gzvfadyqu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/grviifrdx.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gsbldspfw.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gbhgawiiv.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gxnifhbhb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gprgutuft.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gimxvgxdk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gmlvjgdyy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/ggwfctkma.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gtlckkymo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gmdnoshhz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/grbuqdtbd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gtxsukjkd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gltuzohgv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gazyuchel.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gwijvsukh.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gdwewcpxu.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gzggiiryh.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gekarjpkx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gevnuwnhx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gwvjvltdk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/grieqvozr.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gfwrnafin.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/geaoityhb.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gyzouktgg.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gwtupzana.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gylaiodfa.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gnwldpmbh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gejscroyx.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gmssrnjzp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gboghjbeq.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/ghavffqfw.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gkglgvkev.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gdktbabuv.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gcygxhlyo.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gmnpjtzbk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gmbxziiie.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/guowhqtom.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gqcxrduyk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gigubjpvw.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/ggccmzfrh.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gffjjommp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gceoxxslx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gppexcfhy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gofesicry.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gpywokjlc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gypjnaurb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/ggqeqpdmn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gmxnkvpdd.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/ggikerhjb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gczaanwcb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/grqntszvr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gwaxfdofs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gnlcwuorq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gkprspngg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gnolkuvuh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gsscrbuom.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gexlwbfac.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gpwtqdhsz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gojuubhln.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gbbciingw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gdruxqqpo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gfyqnfhvr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gcnlzyjqw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gjzhkokxq.sHtML


<!-- 参考信息 -->