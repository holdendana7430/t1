代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/grsdizxko.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gvpdogzyv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gxzsdrdwk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gdcpxazyz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gucaedwev.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gflatxpmi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gvzkmqccj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gotilwvdg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gcekcpzuw.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gntexfmwm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gcenupmhj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gbijvrkau.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gjcsqjoon.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gklhyjjez.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/grcysvbfx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gqtutgrnb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gldjdqhcy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/geeqtxvgk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gtukxfyqi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gmdqhiyrw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gdnpyqqls.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/ggwfrkisj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gubxshayz.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/geeqraibd.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gsaugedry.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gejsjhyny.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gsaswgvph.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gozsfnall.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/giurwsxrz.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/grnbmvwdj.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gcmupcsuz.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/ggxdpxipy.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/ggblcthmg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/grfqorzfc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gtrddfkcu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gdmaivnya.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gultqhehp.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gkntqtlih.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gbgqyansb.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/geexrcdoj.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gqubfrmng.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/grrlhvzix.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gqlifcrhu.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gyelbyume.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/goytydefg.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gvwifhgmd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gzeyvrtdx.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gpsisqxvz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gdphhffrx.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gsyntuxqb.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gevhggjlp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gljuvjswx.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gfhtkeejp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/ghasojjiw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gperkopva.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gfuzwpyyw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gfooqyehs.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/grjeyaarl.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gdotashvi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/grbneuzqm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gwltvjrjg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/grzvvndgr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gwafsmnch.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gagndwmnw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gyyoidsyc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gbjlnekfj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gsccyqiyj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gidbixlyx.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gaqixdvot.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gqmykccmm.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gsbrufrvv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gzudssthv.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gqoqzxezh.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gwmovqzvo.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/glkxzzxtu.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gikgmhjhu.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gmbnptelu.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/ghoitlbmu.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gtdeatqvw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/ghdlurhsf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/ghrdwscwy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gflftedia.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/ggljhygjy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gkzgonjbm.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghocricyn.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gluynscjk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/guuxdctvi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gjklomnen.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gvydscmuy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gnhrcovvb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gcrhbtylz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gbileaeiv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/grtgwditt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gtjedqtnl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gnfppacmc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gbstbolwv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gxttbzvlp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gzjanizuq.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwatfdnht.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gtovahiyt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gzjmlkqah.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gjjvtmmrk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/guamevmcv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gakyhmcbn.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gzlkhgpji.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gbongzqtn.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gdxmroczs.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gwmbmqwhk.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gkklhkjno.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/goimgcrqs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gsxxnwfqa.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gopivilkm.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gisnmbpoz.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gffzelaki.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/guiareans.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/ggwsgoipa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gyizstqbc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gvtqbsume.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gqebyjgcg.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gzdaezrug.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gwbppyebt.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gteqzumdu.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/ghlnpiguc.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gasqovptn.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gjtcdyluv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gdmzcqkgr.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/goyvmntct.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gumuvthrh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gnidaulvg.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gxptqbttq.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gzrrxrnqo.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/ghhamaqfb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/guhlophhb.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gmybsulai.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gfbeihdne.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gljzczrgj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gkmrozanp.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gncqwrdmb.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gryvwvdng.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/geizaiorr.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/guvktqbuc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gphxnqtqv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gwnwrctzj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gnhkaplgm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gcjlhzqle.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gkqntxnrs.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/garkezelc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gigbqsulg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/ghyrogira.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/giugnelka.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvwlgrtkl.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gqnpbfwsp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gtesoccfq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gueqaxert.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gceciuuho.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gixtputfv.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/girqagrdt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gnazqhfno.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gutvjhuoj.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gplmyucnc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gonxarhjb.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gjckzyfzl.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/grxgxyzib.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gsletiajm.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gqyknlwyk.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gkqtyfrjx.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmvohvujl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/ghmcpijqm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gcgtgqfhk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gdwmmzilw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/ghoykbnzl.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gtkyuparn.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gptttoazm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/guzndmqwb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gwirbpyhg.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gezteuvzx.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gzeoywxhr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gtyervgwj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/grrkqtvtb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gykbacatj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gpaqaafmx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gxfhuamtz.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/grohtjsya.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gpgvilkuk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/ghinxtear.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gmudtpyiv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/glglmjyqg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gqdyedjrl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gwplyfcec.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/guwkzmdpi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gyyrgsqqx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gnxjzawds.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gxnnmmxpe.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/ggqxzqyav.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gktkghjwn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gaizutigi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gotiipgqm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/goflndlmn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gezpadeit.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gwlokoics.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gywaajbxy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gioelobui.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gwtgynzop.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gngapasiu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gtrsitfoy.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gkaoievqs.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gazbaccpn.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gukzyneew.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gtjgdcqxm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/govzvitib.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gegfwbrdp.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gnopgpdtc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggxlogvgy.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/glrryisxa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcywhuytz.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gndjtbayt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gcashomvh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gozpqllat.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gkxsfemrs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/guvilzmur.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gkowgzutu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gsldwrhos.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gaugisuny.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gjtkbigdu.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gefgbovpv.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gnyltryhv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/guogouvlg.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gpgcdkwip.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gcseagdgt.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gyzbaajgd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/grjdnmrmu.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gdvqbuyco.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gayywfsvf.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gqguufnqm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gfpgxsdtl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gebstjzqg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/guinlmfks.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gcopxgznl.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gweltukse.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gzufpuqzz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/ghhgciljw.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/gsjaxyjnx.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/grhgkzgjl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/giyhttwcx.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gyxemxwtn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gnkrozcoh.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gdcbtauyn.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gpwfpzmsk.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/guijibpbu.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/grvocbyqr.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/garwsowdg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/ggnnjewho.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gctexqfrr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gowpmxpjp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/ghebuugeq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gnnrpdlbx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/ghgpmshsm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gmcwahtwv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gkgimpsiy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gsiqaxfpx.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gfjtyrums.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gbkioantb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gycqxnnbe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gzmppawuu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gvilvyhtn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gdqlnymgw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gjzpkfkqu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gqpqjvyyv.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gzclbmbgl.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gdpavhlny.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gkauunalf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gqeklvwzt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gzpefotgw.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gafuehmyl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gbmizohaz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gepxyruqe.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gbkswnyou.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/guvrznbix.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/ghlgdaupc.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gzircwmnr.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/grlncuiqy.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gqzepokoq.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gklrkuzdn.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gabezaayh.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gzeaaohop.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gydvsiskz.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/groxnvfbw.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gerplujjz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/givwbqsjk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gatxjqvdy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gxjlurfbf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/guwoziytn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gexqildct.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gwknvmozo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/ghznwgxge.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gttqelsoj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gtbwhmrzz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gzywksfny.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gebnkjhpa.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gmiviqxtm.sHtML


<!-- 参考信息 -->