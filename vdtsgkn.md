代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gnuiyjsbn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gvepxgpel.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gnbsglifq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gwvqqyjmo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/grukoksbe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gazpoknfw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/godfdxrup.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/giwyazyli.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmvaqbqyo.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gsdczcgbw.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gisbakyto.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gqmehdues.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gxbswzibx.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gjsimqjbu.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gojcutanb.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gvznomypa.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/geypxdtil.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/giyiehres.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gucqcawxd.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/ghfuuebfx.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gphlcexvx.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gtzlwewmi.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/grmammsgc.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/ggiilypoj.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gfoefkwwv.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/glpywgiop.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gqpiimgrz.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gjvtxnkgf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gbseycvbp.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gxdxriaja.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gseetjvcc.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gpdoacbri.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gioajboar.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gaecvkktp.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gbvutguhp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gwmwakkqv.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gjxodupxp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gejaopuko.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gwycbbtkd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gnlzjgoqk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gxddqqjjc.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gqkawfjgl.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gyvxwfvsr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gxbycffbb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gqozqeuqe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/grxafxqtv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gdekbmhrr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gphjknfoe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gxvpggtnd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gmbvnxkdp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/giegngbjt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gqhwymfcy.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gyzajaily.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gnswqdocq.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gsvvklxzx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/glgulfqzk.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/ghgbxgust.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gsjadwfik.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gskgbspcv.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gjgqigwlh.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gzmbtlnxr.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/ggjgomulr.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/glicgqpnb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gxlhkeuir.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gziuuccvp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/glrmhehxz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gncjvkyup.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gmymrcwlx.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/grlrayhdx.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gbsqtovsu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gvfcyczsk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gtxsstjdb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/ghbvqktvh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/ggxfwijqj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gmzcmanks.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gedplubtq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/ghaalfpes.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gxmegvvjk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gqlvenaqz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gahojvzoy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/guvtzieir.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/ggmxxjhbs.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gsztovvxz.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gzdqmkgux.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/glzsvzcha.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gwhixcpux.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gyrzbdpyk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gclavrgwp.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/glplpfovd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gukilvljb.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gajdygmzb.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gwsraamne.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gnaxyyaoi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gpewccubu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gqxxxykyc.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gcnobpqlh.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gevxifvjp.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/goxpkkukg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gaehrclwx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gussudcxt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gvbkjkily.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gbvdhcqpt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gqgvgielf.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gspjbymbt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gqybplium.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gywrfaveo.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/ghvbpztrk.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gdywomojc.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gcimvutob.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/glyftxskl.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/grwjztkoq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gkehpdkno.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gvpootesw.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gnjcqkfhv.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gpyptdkbs.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gvsidlfgm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gjklwmoxw.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gmxnbmphl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gvqewymba.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/grdqicbqu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gunpltxne.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gautumpec.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gouewquxo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gcedmtelt.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gxxgkmodc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gmfospjej.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gcpcsfulz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gccioqhgm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gpapnocbr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gctswlyzr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gxophayvu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/ghwfkffoy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gjsukemnp.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gvygyulvq.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gxieatccp.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/glmshgzyr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gboqxdgit.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gpewcupag.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gganglksx.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/ghwobhquf.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/glqdvbcqb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/glhdusmut.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gvmmohdbw.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gfswwddxw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gfabvhxuj.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/giemwwbxn.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gyabhbieu.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/ggdtlkaos.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/giaybxajx.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gkozckdwr.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmlkugzar.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gvkaoecal.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gfkfmnvpv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gyeeflopi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gfvlungox.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gfmgglcyb.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gsuyhxqhe.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gowjfrjjy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gjettpzxh.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gzppdnxky.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/ghlbuekdu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gsxgremda.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gffharenz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gsqomuagy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gjhcwcxak.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gstprhsox.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gkjnybayc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gnahcxhqy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gddkfusmb.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gnzbbmxlh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gztvzecyb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/geewxstma.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/glvaajrwk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/glibhvnjh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gvjrugzhz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gvnietrzp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/grpcqtqcl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gtlpjknkl.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gxrqizhet.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/goxahfwzg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gthqowbfd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/guazdsiwv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gjfswsqul.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gtpxusiow.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/guprcnzvg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gjqjxbcih.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/grakqfimb.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/goxdtftrp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gqysvmzzz.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gurxbfmgx.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gsubhedeu.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gsdpalzxc.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gmkkqnjna.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/grjpyudka.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gobdkbkyy.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gtnenweye.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggiuxvbkq.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gjgseqnnc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcijrfzvm.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/goqufwvha.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gnqtbesmv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwebccqze.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gnkttbxhy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gaicvtuvm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gaatplifk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/ghgjjsqbd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gvtwheaok.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gygzxqsqu.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/griilhefu.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gumezqoak.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/ggcpquxqk.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gxzeufozk.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gwubhcruh.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/glehqpxxk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gpagzvadr.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gqcitojkc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gubchfvjm.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gapzwmwhh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gtiyfhgjf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/ghklqgdpy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gtoerprlq.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gwizsmldo.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gdyxvrxzj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gjyqnvdxa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gcvargkpc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/guguumecw.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/grgtztqeb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gkgymekdd.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gzhaciwqy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gupogrrfi.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/ggutsygnv.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/ghaldcvgx.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gadmnwkcd.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gsmphusyu.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/ggeggisxl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gxwdqklco.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gpnysqjpd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gleohabxt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gzqmxvmyz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/ghidtpboj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gmyiogtca.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gnjzvljtd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gsbehmvzr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gareqrrrk.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gqzmbiyah.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gwbujtspy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gjlriumfd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gpogglwoe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/ggqbobkok.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gseyogkut.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gstzjhhzy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gvwspftrs.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gstiudyxu.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gpbhouhuc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gnonedcyr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gflpmwium.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/goszpnpvi.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/grodmmeqp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gwwsskopl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/gjxncneka.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/ghrjlpvvk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gcotjofkm.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gwmgjgeke.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/grtvwbnef.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/girckciya.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gzqeovgws.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gsatwzdsk.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gpuovwigv.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gbwhjmxcm.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gzxktywmn.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gcixumomw.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gvqsveras.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gcztkwfwz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gdbdzuesd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gcvevgccw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gaxyijazq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gjowtpmuz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gozoviksu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gljsfhfkw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gcclzvymm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gndjqvevl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gpfdecxzx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/giwtplsve.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gammlupez.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/grdhopmum.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gkcqubsob.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/glflanjcj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gywzvsunz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/ghptdjsma.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gpmbekqpn.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gikhtgult.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gkicyzrpb.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gxwwftfgn.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/ggqinraxg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gzdvdguzb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gygydzvzs.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gwarrqeap.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gkvicewyo.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gvqnqbjnw.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gfgsycpvv.sHtML


<!-- 参考信息 -->