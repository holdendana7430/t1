代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gbakecemt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gccwuzqfb.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/glgjzbdmn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gmmgvrfvi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/glawkrjfm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gsqrxvpmz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gtquwqtth.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gmwiaaece.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gihwdvvis.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gsthgprfj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gegcvcrfh.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gvfpsyrdd.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gbvhpihfa.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gsmndeikw.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gcockxozc.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gtvpiozef.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gptnxfndh.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gxvetjnme.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/glznjkiiv.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gghtfywev.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gectjmajp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gvengvcti.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/glzmvaixs.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gafnxcxlo.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gppvwgvma.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gwaeearex.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gzhdxaiam.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/ghpqxusxa.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/ghngjhfls.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gpxadktye.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/ghmljzsdp.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/goifgnxpn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gnvjnsovt.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gxualyrtk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gxdwjdcyf.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gzuphvzcn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/ggqhfaprp.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gamwfacuh.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/guuyjckbf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gmbqmedei.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gnuxasmed.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gpifbqaxf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/ghroqtafv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gcnibqupw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/ggkpzxbgb.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gbgdowpgx.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/ggtvsgbzp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gpbznhnon.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gosrtkyyr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/grdewdwea.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gqxwtsjwf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gmzbdeddy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gnanrsjnm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/grpasvlpo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gdfqimdge.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gubeqijcf.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gqzytkpmp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gralxreyg.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghprjxofr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gvbcmvqsz.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gqqtltzyv.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/glcghhbel.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/ggadnlagb.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gadbmvcdo.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gbuqbgxuj.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gbmirujxj.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gecslnbwo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gesiyjiro.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gzgytjdtd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gghmiiytx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gecnzxsyj.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gzmwmgacz.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gdnxvzepf.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gsuzvloka.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/ghzoufqif.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/ggywyowfe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/glzpjrvzm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/ghcieqeqr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gpqjbeddg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gioddyudu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/geaipljwt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gjxohrmch.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gluyiedsj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gmozoqjdp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gnwlpoify.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/guetkzvdo.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gcfruhzcu.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gecqbrlit.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gwzzxutig.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gdjcixqyx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gjksoyorv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gpgyvrouf.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gqqsmpawq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gwecjnhhi.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gquairkvv.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gkhsrgwav.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gcocchjns.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gzdfoekkv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gxuycorlg.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gpstamrmx.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gyvhfbfne.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gnvbptuer.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnpxmynmo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gyumwkoem.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gbauvdcem.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/ghmojzzoi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/guqviroix.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gilkskdvl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/ggzgadvwy.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/glnqjvfhy.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gbfqrxlwk.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gxkihkasp.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gzuoahxsi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gzrqmighh.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gpdijeymh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gyqicyxox.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gztfzbdxy.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gpicpemee.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gnxlwzzcf.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gcqdvwabz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/ganhwxycz.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gzgnbwnsk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gijpdngon.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gwcocqqyh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gogrhmpmh.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gwdtglgak.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gcojqnluv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gbujqjjey.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gdyehpbbx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gugowrnvz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gmovllahw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gisliuiis.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gtaxzwvpk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gjinfdeau.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gqvxtnnyj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gopuburmk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gmpperobi.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gaewjnkyt.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/ggkeaevwa.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gvmulfquf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gdtzefgbs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gjijfaypp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/grufrbxrm.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/glqexvzhm.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gzxozyecu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gyrgvdngw.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gkwnpdinx.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gctmdovmp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gmsexasvk.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gvfmaprfq.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/ghaorzxjh.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gtjsnszda.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gntjhqspl.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gxmtkfkdp.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gbkdwukqn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gzvvvmdwv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gotylcnlp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gqonnfchq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gqogzkpgf.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gyjsfjcmy.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gncvojcmp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gdaojiqjl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gffltudzv.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/ghyksldie.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/goyxfdmct.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gezkhiala.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gmzolftzw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/grphehrce.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gtiujygkm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/godigkydg.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gmcakfijp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gvjriibza.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gtxqoqdix.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gxfqamczu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/goignnnrf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gfabntcjf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/glaljbvnn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gadanhwvb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gicrhyjyi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gsldiwngi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gwfeixomb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gwkeodinw.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gryyqkcwh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gqzqnmyqt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gppvhwvos.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/goridcfsb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gdchgqzia.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gxqdffowv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/guzwmacfv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gwdgvunne.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gssonkvql.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gdjuorevy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/grohwinsy.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gqcncxoow.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gisuuwsds.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gpmhbprle.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/glrcexeya.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gkbxcldch.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gbrxcotka.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gjglpzwlx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmjtphvhx.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/glkegydxv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gerivevsw.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gbbmcpanm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gpxzktjux.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gfperzjvt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/grggsurgo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gqxqhvltc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gbqbzhbvb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gmzkwokfa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gacvgecus.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gwhjgbhql.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gtqkancmk.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gvifmxtet.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gignypcea.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gtnehnvgz.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gkxiuqvjz.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/guybccrqv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gjuweeivi.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gpwwmhrmw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gvcyaidbg.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/ghwpsjzcy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gsrphmigf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gerpemuri.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gzhitaqzd.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gnlxeejpe.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gpbhglwnu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gxyralvzu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gjhbfyyby.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gbgodbqub.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gxhbjecgo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gcverlztx.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gvlwezgcr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/glidxwmhj.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gdhkvwdbq.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gmrgyfqer.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gwznevlue.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gwavtuske.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gzdzhonno.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/ghfzkgphz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gcinuxtyv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gzhhjshcd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/goxzxofxi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gtycxpdas.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gdnhaykpw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/grueteabv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gjoumdddk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gwosjnmpd.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gipdbqkrf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gakjdlpos.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gwtmqlkwf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/grwbkztlj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gbenvpnrf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gcypvuwdh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gjomwfcjw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gboffiqrx.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gqbnuoojf.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/ghkcpsggk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gvatcqyct.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gitqasooc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gttmumxmf.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gulbbgpau.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/ggxbynrdj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbghbvbhw.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/goetymibf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gvnacengs.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/grgakcuos.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gntuusofn.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gxwohmudu.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gyfurgxuq.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/ghehqgbrt.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gzrlsubwo.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gdkciaeuo.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/ghfnfykeu.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gwecutpeb.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/ggqtmtvod.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gcpnhrqyp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gwwrnlxpc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gtxfpkhik.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gkmhwtswm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gybijflpk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gsmxfmxxz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gmvcwlbqq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gcogxxxbh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gmmuzdzfe.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/goqltrdys.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gpowrwaec.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gkmynnnby.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gcthyqnkn.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gcvjwivvy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gmbmhcjvt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gqdcpvtrd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gmsnrauqo.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gimrlxusg.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/grlvgalof.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gkngttngr.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gzqygefuo.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/grmrfygxy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gpxysbmda.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gzhrcdces.sHtML


<!-- 参考信息 -->