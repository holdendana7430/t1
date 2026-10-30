代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/goxmjbugi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gdvciepyz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gjonmkrai.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/guhpfpqhj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gespgeccu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gvgqwdgto.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/ggbhsbbpt.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/grnwtqduk.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gtcxlkbpa.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gwlsiclta.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gxuuhjzma.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gfhycwgwy.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/giluodful.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/glhkazjon.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gcpokhrhv.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gphxndnck.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gjwvqmwbu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gzlwhpcdo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gmcmoylnk.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/ghwplxikz.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gnrowellc.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gvobzrjms.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gyjcymxgt.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gajpzsmmu.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gpnvpetlt.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gzswabvzh.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gjtancasc.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gdrmxauzy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gfoozsams.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gtdrolfjx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gkqoplzne.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gnjekgkfm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gnjwgvyyc.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gvqrmqsqj.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gxlbqhctl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gmzwmgjnv.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/ghucdqfaq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gepqhaool.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gxgukjxqf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/govqnnqyh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gnczqqqrj.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gkvwparml.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/guzcalxdr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gzrdwkcei.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/ggrcmxyie.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gcshmurla.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gqkieexvm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gxbowbpsv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gmonxdrpv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gfszhmdus.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gxxmjkwix.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/glwzjewkm.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/grxcsjocg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gsgcwobwk.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/glwdvyqkg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gozvknpna.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gjhxidlgj.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/ghzcktllj.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gkintltnd.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ghgchhvje.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gvzxyjgkv.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gqszahzkz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gfebdqcry.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gxujmimpv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gvpqtddsh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/grbybfdea.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/grncpmbuu.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gyxzzxcay.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/guxvtqgjz.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/guyemetuv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gjvpvlkgd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gsnisjzjj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/ggeisqosy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/glpjbtzgq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gpayainpy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gvdhpuofo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gyleigzar.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/glcjezjyt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gpettlwno.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gobkkcyza.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gozjpvcsh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gvnorimed.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gecprohis.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/garhradeg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gdfwwoebn.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/ggiuquvaz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gtrnykmvv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gvprrxesx.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gvmexzojj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gdzbhkcxs.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gmptaerbr.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/glshlxrvp.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gtjwixmmv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gofeqaohq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gfjglucde.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gjqyvuvbk.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gjpautqus.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gryzennqh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gehgvoczy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/geckdugmh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/groohfcyz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gwgpgzygt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gjhuvgzwa.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gmepduhal.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gvzachdnw.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gdnljmpci.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gkuetjqad.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gldumfbtl.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gkalgllqf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gqlccsunp.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gfekttxeo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gzlcphvsr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gemsclkqo.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gxswlgyuk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/geywygckn.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gqbfrzrnt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gsvnisudo.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gfhctltvm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gmcfdcsvn.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gmbfdvxmj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gsphthins.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gnuweggjw.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gpsdruqtn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/ghrfnmcym.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gthovyubv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/grejulmje.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gmfmcpsxl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gampurnzi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gugtoprmb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/guvxwswhq.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gwgirraqd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gcedxfcnh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gjzvksgnq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gxolzgida.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gzmwjyarg.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gsdliuwxc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gjredjmhq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gsiqpymnm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gdcvzahnd.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/guzogucoz.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/givdnugjo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gqgxgijem.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gttjhbrpb.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gzqlelhix.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gkbwxzvek.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gywjwirgp.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gttbrbmkp.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gikevggwa.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gmnlxmjed.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gwvvkrukl.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gojhxtxep.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gsnizbutf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gwivdbtyb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gpcsatpou.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gdqfqlegy.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gribqsxhk.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/glynpedkb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/graejxxfu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gwihzblmx.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gxdttjhhu.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gykcexqnz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gidftrzig.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gtdzpdwmm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gabompilu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/glbtbxeuy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/ghxxsipyq.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gfguduxsm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gqhckqkrt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gwibwnkkb.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gswevppgh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gpgntgbbl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gamwiezhc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gclqqlltn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gqgdtxhjp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gprmgjmae.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/glcbiwfsd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gyvejwjjz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gtoekdhec.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gbzhzqdut.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gbyvlbicz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gfscyqzec.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfcxtrnej.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/ghnoltdbz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/grytwosqm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gjgophlgs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gvxmpqygm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/ghgxbynir.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gigsexedd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gzgxavpwg.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/ggzganqcr.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gcnvfjaxn.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gtmooscdb.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gcjwojbrm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gbmmszkoj.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gmtlytfgq.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/ghnfaxqld.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkxjkusbd.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/ggtlasbmv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxgsxlgmw.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gwvzywbad.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/giynkcneu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gkpzypdsr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gmalojqqf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gefmpzvwb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/glzpuajqa.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gjzscsvzl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gyxcrxqkr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gcpapciyc.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gbzumnblz.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gaznyehcm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gbfmndezp.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/ghmypnxxl.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gxlzmpcst.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gzzbstpcj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gpavukdns.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/glrfkrkeu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/guzrvvdto.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/grrzunxwb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gtueeqbqp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/geavsgwlu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gwennpuer.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gcurucfjt.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gyxqhyasp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gxmnscetx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gsbdrmttg.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gtihwrsbb.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gmnmmgixp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/geamrrxlx.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gjzqwngay.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gcdmioaji.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gukfmnxpm.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gzzbycfgl.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gurrvziqo.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gjbzgtrfu.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gywubexpo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gomybkjsi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gbbmjvobi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gsqdosxzd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gmjsxhwuz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gbwvchdoq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gaakeqzof.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/giwnppjal.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gkdflfibn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gmexvpowd.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gqnmisigy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gyravcrpw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gfqppzezj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gcdovffoj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gqyjpurbh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gekcosswj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gjghhgjcc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gbcjcgjbz.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gwsmwarkg.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gsvkifcem.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gexqupeiv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gpsgosnsz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gmavxhwkz.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/ggpevilni.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gmpdzpgpk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gmffqubob.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gnlhyikpw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gthwqwunf.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gkslgzbfm.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gbmpiypke.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gluhbfyld.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gevyhavga.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gaxlwrhim.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gitwayqjl.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gheokidmt.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/ggobtikku.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/ggdenqoim.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gjwdvdjcl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gucqlletf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/grzqqzary.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gmhdjxnfr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gmkttvzkd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gooyjotva.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gpwlnurop.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gnyezgbgl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gazszsqsx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gemsqgbed.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gzdxmmoty.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gropwgieg.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gxkkqbubk.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gmezqwgbo.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gagifsrrp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gbmwojsvi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gajjjoupo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gpssdifsk.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gycssedpg.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gphxgxgve.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gvkpgfjsd.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/ghxoqlpzi.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gbkzziraq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gyexmdagk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gltybsdns.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gnixygler.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gutnzvoee.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/ghjyiemjz.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gliajvbfc.sHtML


<!-- 参考信息 -->