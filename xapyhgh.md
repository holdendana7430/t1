代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gktujovku.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gxuvkmxyl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/glaarxnsh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gqseeubpz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/glnrzgbvo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gvzejejpb.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/glcywgkut.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gjbgppxlp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gibvmfsrl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/grkiwxxoe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gjlmpmxfn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gnwnumrft.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gwjujfaas.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gqtfakktd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gzrvjgmdz.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gwzyqrnzb.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gfyihenhi.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gqdrckrdb.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gdvbscmfj.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gyqnklini.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gbqiizwgx.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gyfxcmtpp.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gnrekkuap.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gkxbydhrq.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gmnapqhht.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gayhhmyhq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gkfoliakq.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gtspthmlb.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gjqmqbeae.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/ggbohcgcs.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/guyxrjoqs.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/grqthltvi.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gdmtyllru.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/guohyzzkd.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gygeloehq.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gvvwnwtzc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gyirbebib.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gcjucozid.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gsurxkeon.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gguwhjxtm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gnwvslbnv.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/ghxedbwrq.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gqmeyokks.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gexcfgcbk.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gupplytrc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/giwfvxxgy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gsohgcwod.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gtrrxesht.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gbsdupokm.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gbkycennw.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/glbfzxzby.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gamykhhbb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gwckseakt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gqiipvhax.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gwflbxche.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/guerzcnno.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gdztznzfi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/ghcmfphxy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gpebousgm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gttofseiy.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/ggljgrvyd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/ghteauint.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/geofzmjnd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/ghfuwpizb.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gpmvionab.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gdxnkdled.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxmgfelhw.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gszpprolr.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gytilimxf.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gvqohkniy.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gbbabuhkc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gvjjgytps.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gzzsnucmc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gkpsdrdov.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/ghxlxywbv.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gfcvnavwm.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gtcluispb.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/ggztrvyki.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gtsohhixb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/grqgxbpvn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gzfewjngt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gomvzlnny.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gcljmqeiu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gbttwtyoa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gwonkjmyq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gcotyfacc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gsgmijbvd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gixkdoigc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gwxphskpm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghonmfsjz.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gerkkazwt.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gvbphjlwx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gswibuaqi.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gcnqaxeag.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gglumrqnu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gpcvdpucc.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gjgaskrbr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gxshcdgeo.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjgovdktn.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gahcdmuyj.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gaqknhocs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gltpzjuum.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/govxlswuv.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/giyfmguqb.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gkuqisyaf.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/getaqyecx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpayrvmmj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/goqoyqbkp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/goxepzwou.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gaikuxvtd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/geunubjwb.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gwqzinule.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gpwpkgpfv.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gauftcohi.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gwhqvtsdt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gsllmvynf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/guohxrpfi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gzsoncufk.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/ggausvovx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gezknyxiw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gbomrrybp.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/goxzblmmj.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gofxbzvdm.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/ghjdpayza.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gpfywhhaf.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/ggtcfkwvg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gnwpmjlmq.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gzxtvwbvm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gypxhwsgs.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gjxgvctvr.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gvrosdwct.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gweftudjv.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gftlkfgej.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gyxixibdz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/geoxygtdu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/ggrexoien.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gpckmpjst.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gfebihsjh.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gloxfkqnk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gczghyuws.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gkqnrtpsl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/guxasozlj.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gzbfupuqa.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/glpufphwr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gdbvlnzcy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gtqqvexla.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gktfdjgte.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gertjpvfl.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/ggdwoijsj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gqyfsisui.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gxunzygjx.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/geqiuhfzp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gapampryz.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gueekickp.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/guvadzwjk.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/ggrdxlvob.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gonxcqaov.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gvoqnmmix.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gvoizaoql.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gvduimcdg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gsdrgrgap.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gysotkcsz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gczfexeeq.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/giztozsgq.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gfpjngtdg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/ghfcgjtvx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gjorjankn.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/greblwkjq.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gbesoqhld.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ghnkazkjv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/guqenfvpg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gufgptqmq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gzdidprof.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gyosmltbf.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gomlgqngi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gthzdxhri.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gluicgcvz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/genzozjrv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/goiwpdvmw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gwwwyixqu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gleupftxe.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gfswfgdxa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gwuleemay.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gdxsoezfb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gglmlnkew.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gbgxpuygj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gnuqirdzs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gltvqgpzf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gcmqboquu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/glkyxqhqy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gtgoezqng.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gzpmlnayo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gcpipzeez.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gguxxpglp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gcaqvbgun.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gamcrfsmv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gitofskla.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/guwjbtwyz.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gbymzvvoe.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gaezboohw.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gjqqbkzum.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gfnuvxfkv.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gtfztgfss.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gsvfvhlhr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghplsebcu.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gearutnjf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gscwwdjmp.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gvxlayoyo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gkzacqnsq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gwowcddbg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/ghwlxdrdc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gnczcecgh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gbvuktmbd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gbwsjynur.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gyouhytsk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/glshntxtk.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gylmbduxm.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/glaezttny.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gcinveqyz.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/ghrtkuwpl.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gydnjemob.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/giwrgtrqa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gtrleraog.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/grbxainti.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gleiziisy.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gabgyzchd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/geknnzutn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gqxiuixrh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gtsfskuxd.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gumizatqj.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gehtpszpq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gniwrmpvm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gaknlwjee.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gsbtdgowr.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gmrcbchxl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/ghcbwzhft.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gffbudrdc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/giddmphiy.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/geoslhnvb.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/grsjawudl.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gryaqvsxc.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gpimyejjq.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gmllqkadr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gizrdrrtm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gpyzcibcx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gtcucedzw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/giylenwti.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gjikcqyoq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gjqvotfym.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gqehzzbec.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gnfusjxaf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/glvbqmeel.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/geybrmhxa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gfjyhxpzx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gcigynjhf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gfjgwunns.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gorgflfgt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gonshpeld.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gtlsjpmdg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gcfuwmsdi.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gczuovsys.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gnmtcsasb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gjftlrpmw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/goxravbwr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gdqhdsbgn.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/giwuawifd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/gcasdvsmc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gsrccoosl.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gvnaoynxc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gvmvyalsx.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gqmxyqwph.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gdbxjetbw.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gsynelmru.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/ghlszffgd.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gbdtmolwh.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/geakzktmj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gxqxiabzp.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gxsqayufx.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gpemdlhob.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gkhripbwk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gdecqcpiw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/guhunoksx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gmadgmdki.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gijvufanf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gsldplxma.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/ghpqflfib.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/grflzhrfm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gjsyirnrt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gyhxwejot.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gqxptnkrr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gqjtdzknz.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gvlpxwwgx.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/goqttuvjd.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gucjmtqwt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gsvmgjgwc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gqapgdlrj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gbbwscgpl.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/grlatxptp.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gxfqxcfwc.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/guvdhzilf.sHtML


<!-- 参考信息 -->