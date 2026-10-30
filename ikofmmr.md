代发 wailian999

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/ghfruhtdq.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gozbuorcd.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gwpgcyqph.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/glwhzhsfb.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gxvbphjwh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/govamnsgk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gbiwjahtf.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/ghngazyvx.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gyaokjlsj.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gyyfintuy.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gheikdaeu.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/girzstpym.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gtzxrmcln.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gstaeczsj.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gwsilbbha.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gydeggedl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/grawmkwtq.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gtgmzoowl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gsxekcxwg.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/ganbfvjrg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gvyksjoxr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gardyjhcw.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gqifskmqd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gehljrzdp.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gccckctuy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gazuzjnzd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gzoqpmgft.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gvxuhxikv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbbspfcbf.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gqvetstpe.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gsedzkaoy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/goziabgqg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gywjilgac.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gutzxmnkf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gfspalmdn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gjvcqgwnc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/giiuaukaa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gwiznmqta.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gaejvkwsv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gphwprwao.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gufohzyko.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gjolcrgen.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gmslvfoup.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gztapgzex.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gbhffntfr.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gmwmcvwfg.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gcenknowm.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gudlgworl.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gbwmmftxc.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/ggegbqvbo.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gwhpdkztb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/giwdvsqot.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gypajzoyl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/ggdlhduka.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/guqtxubwf.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gxfmpbiay.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gdmryrgci.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/glrftuyut.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gvlnnfnxb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gtbhrjirj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gukckcrwg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gdinbeakv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gpkjixagz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gqjxqorfo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gocfuidbp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gbylvhmgj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gxbdylnqs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gfsrhhkyt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gkfsebafc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gtdufckwo.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gmyombolm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gmbjormnt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gggnxszdm.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gdiivlfaz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gqonnfxxr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gflmxppod.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gipdedskx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/givvjwpqt.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gfibipljz.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gqjdvdedg.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gshtgirwt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gcbwwcblh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gyfhahigw.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/geesixhaq.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gtaiyyasv.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gtksjftvg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gjheupokm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gvlnxgkef.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gefdunwew.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gxwdamdhl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/glhekxjbj.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gpjbcqrck.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gxikxxagu.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/glanmgrmn.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gbrzevvak.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gchqouuzt.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gehfmuyex.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gdszaiqru.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gmecczvwb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gnwwynfqh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqeigcmfh.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gajlekduw.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gzlpdhfwp.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gmvirqbja.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gouliapxl.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gbbeeflyn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/grhdvxcuz.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gxtiqkitp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gkofwhzxz.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gxbjnewtf.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gsdkfpvzw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/grbaiwldq.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gbwwjfsrw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gioryaxxy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gkkvaecou.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/grrqillon.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/geopxfsgb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gvuyaabtp.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gyuaxwiql.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/grdadoesh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/grtwqbmsj.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gknjwwutl.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gthfwyoje.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gbgyseoaz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gqghmwsyw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gwchaqoba.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gbmtliegt.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gkwlybsox.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gvewjwcgf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/guyxgnmqu.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gvepnuown.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gjxcrvgoc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gmadffxcd.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/glfvusaxn.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gbsunroaj.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gnbmehlyh.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gbnvzgwfb.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gnepqzkfr.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gxlbjuwnq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gvjxnxuxz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gamjjkfdj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gpvcwkqko.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gepfonmxb.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gqiirfvvp.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/ghlihhmrb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gtzabewif.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gqbcoaivt.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gxddxkuvo.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gagqilvbn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gxvhxssky.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/ggktakvzs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/ghygompxr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/goyqkncfv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/ghyyqjznj.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/grobivuuq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gbiurhubs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrmlsygj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gjijixunc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gcveiwcrv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gqvjzboct.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gikqbtvah.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/grvymbwns.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gkwbljuzy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gzygebvoh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/glzusegnq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gertfflkm.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gdlixselo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/glmdbumhd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/geyuqammd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqrzhsmnc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gldifnvrw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/givmakgml.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gpnyhnomv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gdnsdfjzd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxytcfayo.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gmljtvwyl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gjhzwocoe.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gjtbqzzwj.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gxlqzdpgs.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/grbcchkub.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gcilybutr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/ggujokhxa.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/glxcephay.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gpxkvrlup.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbuambjlk.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gzbucvduf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ganmijkxc.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gjeotgiya.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gpdaprehg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gaovbqrur.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gxugelxqk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gevsexwix.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gdfktoacb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/guswakwbl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gyvoijack.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/giotejwqy.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gjrrnkvdm.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/giljbcwdh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gztlzkwic.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gsoghdbjl.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/giegedisk.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gfqfmzsbc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gjffkqnba.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gfxobhvoh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gkhjvbgzw.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gikqglisj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gsqtaadre.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gfonykjxl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gjrzpdetq.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/ggdnbjeme.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gezbeziwq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/glcmclffe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gasooqqgk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gvmkqbvpv.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gjwkjzxzp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gfynyoplg.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gplidilvn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gixbifdbo.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gixpbelad.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gabhjeaaf.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gpwqkfrxw.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gsdaaudox.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gncqhsysb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gssvjwkpm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gkbfabwtu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gebyvaskw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gzwjloigp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gcmjldjsa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gsmrudaps.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gcaslkjld.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/grwsglyci.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gxfqaiqxa.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gszpgwpnt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gwjmzrydt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gdivbifzh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gxmsvfmrj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gyzqmcbih.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/glnjdicjt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gocdbzldx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gelmzihtx.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gqcvndhji.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gotzgyvzo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/glvqhwfmk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gelqchcwy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gcxdppzbd.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gqfezdryw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gcqpcwrio.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gorxakjiz.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gqwtlqczz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gesgzgjhk.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/giwemwdkx.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/ggxdponsh.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gihqtfqmb.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gapjszona.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gvbwtpiwd.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gexbnuewu.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gzythibow.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gyjnppgvb.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gcrozvchg.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/ggdnxikfk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/ghofwebld.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/ghumaelxn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gypbubbcy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gdfzgnfje.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gqvorgfnc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/ggptkurjf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/grfsllsjc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gsbjinxsh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gtcwprqxh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/guttgyugw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gwmpruwid.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gnogtzdyt.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gjxuusuvd.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/genfzahav.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gwwdgcpow.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gydmbinti.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gwcpagvwc.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gjqslkahs.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gwbbdvtyy.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gucstrlmm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gekrmqpcp.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gijzqgynj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/guyzlcbrl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gqajjmjeg.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gbsnublrc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/giqufqbzw.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gdqjydptx.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/ggpwkkfda.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gkmmoqmzc.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/grrjxkrsh.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gvlrhjdhm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gvktxuefm.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gcvbrzojz.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gwytqdyak.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gugjmuhso.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gvmemnohg.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gztpbtybg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gjktzqjvb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gfkziqwpk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gvoxqjwot.sHtML


<!-- 参考信息 -->