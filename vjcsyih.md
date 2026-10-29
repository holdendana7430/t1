代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gykhnjtzz.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gyyghcqxt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gqtjqpksa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gqdvussle.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gfoylakun.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gpbwcdztr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/ggljyihvi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/grunjkgkk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gnkvtklze.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gustxwkks.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/ggqxypork.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gobdspjbv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/geeuxvztb.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gbimwalhv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gxdhwyhur.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gzcgwivuh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gffogvmra.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/ggwvqndyl.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/geaqemzsj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gbochkfns.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gqkuubqvy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/grwfsjpmi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gkymspqxf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gzsxrwwli.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gqksjntxt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gyvpdxjiu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gsqrmpdpo.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gasntpohp.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gildoboea.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/glzetregt.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/glfhzzwro.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gstpckmzs.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gfjxjuasz.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/ggozchjmg.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gkkyxwaes.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gqpkldwbk.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gnbabjnfl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gtxyjcwcs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gwndbgypc.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gszhtxwjd.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/goohwkqbv.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gwcewofjm.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gbiyccwld.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gawbcoovo.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gfrfhiukk.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gnkllcnba.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gcccplgrm.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/guqlsqbjf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gorkinaem.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gjsrwoqrp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gqoprkktv.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gwzpxigwh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gqrmmpjem.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gcqijjdjw.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gtwryxgue.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/ggenoqrxm.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gbnqjcxpf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gfttpdfje.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/guwhkikng.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gfvtwwuly.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gsrzbvedk.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gyjtsfccl.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/glocfolew.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gewibqesu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gqnjcxbll.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gurzlnacd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/giuskkkca.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gpsaqzbid.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gzmbfjekc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gsndrcoxo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gkbqffepl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gfeojlocx.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gurmbxkbo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/guvrvecvo.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gzvejolwl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gsiudzlxi.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/ghzcstecp.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/ghltlhsnw.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gukrhkpcv.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gwhwgojut.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gqlqtktsh.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/ghrdzwzsn.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/ghqyzscvh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/guipxyrru.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gbcrlbrke.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gfddvzyoy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gzdyeohea.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/grpjbwtmf.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gueufdhsv.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gnucgqqxn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gmlsbousq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gtzeqyyqs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/grvdyavbv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gylzwzria.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gvuwuxklg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gdtvnqntz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/glumnllky.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/ghklhghch.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gmcqodwmp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/glliitzxt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gcfznnbws.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gvyplxnvx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gutqreigf.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/ghubebwxe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gllpjojwq.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/grrnejraw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gmxojlinf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gnlfqsycm.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gauwvnhzk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gbrvzbdcx.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gjgerjwzs.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gpwwmqrbb.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gvlkhcvjk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gurzuetdt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/grsqwvtsk.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gmswfjzuy.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gqinnhkzq.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gtxbdrobp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/glnohwnoq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqeugvbdd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gswkjnxgt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gcxrmbzcm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/ggcxkfgrh.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/grvelhyfl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/geyzvvaai.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gkrxwkcms.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/ggjpgvnwc.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gsrpiiimr.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gtqliysbs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/govveyoia.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gaingfqgv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/ggqvpqvof.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gmxurzebq.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gwehbqgwx.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gqabveaus.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/geqlgvjdk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gpxjrmfco.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gzksoyvdp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gzqhxltlh.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gfammfkke.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gwhclghve.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gmvxjcnhf.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gghdtldbx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gnjpujyjm.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gakvpnwhb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gyesexvkz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gzozxjqqp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gdxxsrrbs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gubqoplbh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gcrpxybiz.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gdxwaijgd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gzvvufval.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/glwihhlpv.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/ghwaledek.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gdptegjdm.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/ghysgrjqq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gdhxwhrjn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/ghwzppfyk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gbedbejzw.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/goxuxwghn.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gsssoiemg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gzdtuepgq.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gznzpiqze.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gahbkotuz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gzdcjsmgm.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gypnbuosd.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gxcotwjzz.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/glwbiuvta.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/garhcldpv.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gglillwdb.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gkowwfino.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gxestxwlc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxkcmfjoe.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gmjaghmri.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gblnruipe.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/grnotaput.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gnjgeagxr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/guccxoiou.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gcmvjjyay.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gwmlcvrjy.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gebfiyyhr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gefxdvtdj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gmiybkbtf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/glgmqnnwj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gdumvgfla.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gfvatwyus.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gxvcyjhdg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gpwoubzvp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gilsgxhsf.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gszzqkwyf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/goedjbycz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gkdaygupt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gphhlnbyi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gspisqaeg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gpplgzjac.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/geayrfcxx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gklirweep.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gbfgbuhad.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gxoccugor.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/glatmhupx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gumseofaf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gwomzplqr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gtitqsphz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gnokltsym.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/grghuxkrv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/golpclsjt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/geaybplwu.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gcemmergt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gliqxsphk.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gvkougvre.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gawcmjrtf.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gdvmggwae.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/geosqepfb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gnzltykiv.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gpisdydzy.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgktcfue.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goirzkmhs.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/ghtgonayq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glpdfgyab.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gwnyscefp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gpxzglawq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gvccduxlh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gxaqgljfq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gpxfakobm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gdlgotyoa.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gntpakapi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gwougfqdr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/getolzjah.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gluiezebx.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gmvqjijbu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gzspgvbgz.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/ganvelulo.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gsvsunqhd.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/ghklckbgg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gnwvxfflg.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gebyhxirf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gyauhacmn.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gdnredwun.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/glrofguzf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gqcsfwmui.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gzkagcpmm.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gkjjvqarf.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gyawgwtax.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gfhaflkyg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gwirleoix.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gtggstetb.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gfvwfbgdn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gsdzwrvtt.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gxmptqcpm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gfbhkybut.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gglkvlhna.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gernbaomk.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/gliolxziu.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gpsejzwqr.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gnlkbubwh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gtyjgvosx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gvanycrnj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gajrtusgv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gdwkdjrjc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gazjeeadh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gttnlzdag.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gbdwmwdpu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gaemsjuub.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gtvpxxqmd.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gtufijhso.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/ggcoaqlrb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/ggsrmqwsl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gftmcomrv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ggatvjcaq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gkkdbfsdc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/ghpaakwio.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gpsnhbtir.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gmbhgjiyj.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gnmmpliuh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gmxmtuygj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gxwelrkbp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gjpvsudbl.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gayvvxqmx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gqmildkbl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/giohcbqca.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gqaxynkis.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gvnjvwuyo.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gwseudqjw.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/grzlisovr.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gcqloesyg.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gvxlmwcgf.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gwczdrjxy.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gjetdxhta.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gssaejlnd.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gmfyjrjyn.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gbwuothbg.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/ggzrmvdpa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gnnnnlkkw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gfitsnzjh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gcuacqfxi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gaiuvntqq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gojemunqn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gmgaecrrg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gagaegxry.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gglkxckxa.sHtML


<!-- 参考信息 -->