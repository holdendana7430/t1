代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/grkpwimnf.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gdvvszgwv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/ggtcbygsi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/grrdhgkme.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gfndkfhix.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gjrwnlizp.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gnhrrarkc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gdrailory.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gsxqdfapt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gpwdrcypf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gjtbrsaku.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gcmynkqqy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gxpvxlwjy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gipgncjgd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gnvefdkxs.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gorsvbbfs.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gfhzmogey.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gobwalmdg.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gvkaiexsu.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/grcziozpm.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gohsdpusm.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gylwpkdvm.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/ggnzqstyd.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/geaoabtsb.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/ghprghjvp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gnrjzjtkr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gaqepnqpu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gaggsujal.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gzrpcgcbt.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gfwnmjtlb.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/glddsxdtx.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gffgjhghm.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gythvqqsu.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gtzfnigbc.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/giihtyair.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gwefsmkxd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gcyjiygat.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gfxovkbbv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gennsawkb.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gwsywvgza.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gjaukugen.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gibnpqbvs.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gnunxoyuw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gsytuqszk.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/glvkeoidp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gcycvkhsr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gmmcjhdpz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gdegxldfe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gnhsaldlk.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gmtlaobnr.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gypzwogqp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gvccrtcql.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gtifzopaj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gsuyrbjxx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gplqqfxqw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/ghpuzsdoe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/glrmmwzke.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gtklggyip.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gumqgmpgc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gqttdwabe.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/govroazdd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gdivtujee.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gzecdutme.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/grbmtebka.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/genkdukjq.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/ggwifuvsj.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gcngodant.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gpvayfpnr.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gqvkdfwuw.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/ggrlsvevl.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gfnvaaelr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gcuzmvoyo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkslummg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gerbrxyri.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/ggwjysfqy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gcuuaualm.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gbzlvwhyt.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/grfdlemgz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gqtgdbcrh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/glekgkera.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/goihbeenc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gqghtlvkp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gekchqfuq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gccltuoxx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gnoybmuhm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gnphblpzu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gamanzddi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gmobdfssu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gsqfvpuqj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gklsurgbq.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gtwnrtrpf.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gcuylbgtw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/goxzcyvvl.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gfykoxrjr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gccbedded.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/ggfehjtew.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gczmuhpmt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gozbhqbyx.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gylppgzsc.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gzbkdcnhi.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gooeirkve.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gmpxyvypu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gieaaadaz.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gbaphxgaf.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gfrxdjxmm.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gbdlzbrrg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gwhrwqjbi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjrxzbhwt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gwqrrecpy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gseqdlxzj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/ghxwqlljg.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gepkayhgg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/glwjfroik.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/geagzvluo.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gtmmwklok.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gztsavpyb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gkglkifzx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gjkbxtkke.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gbodptvsx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gzxbxexji.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/giedakxve.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gopwidiop.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/glhqmxxkb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gprmwlgti.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gqbfahibc.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gyqzkroyu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gwenzoqwn.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gyfgkkvkl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gajdffnrq.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gnzriccni.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/ggmwrytgg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/ghrdvqmyt.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gidsssoow.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/ghvnpiiio.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gnbmqhvul.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gduuxptjy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gvhmiqrui.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gdnubwkra.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/giqdnmyrk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gzwxdpdgk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gkgwevkfl.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gwfcqnsml.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjinhkcfw.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gruwmsazg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gdnereaqs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gywtlpfov.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/glogwdsdq.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gmocpgjma.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gphsrjced.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gkkdxfvth.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gyihvnwzn.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gagsqyewg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gccegcfyj.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gtymgkphd.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfcuktjx.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gryxempvu.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ggyyennmz.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gdalvyefi.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gvhoabrff.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gaewhzyco.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gfzabhkig.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gdtppymlw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gzxbkkkfv.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gxgzdczef.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gpcacomdv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gubvuongc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gagfyussy.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gshregkhx.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gzjshftvc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gwzvtgdry.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gswilinkj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gcotkxiwu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gfjnfxqpa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gpoxgloam.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gfpoxvnmq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gjzehjkkw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gblgzrlah.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/grzbjqqxf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gybhikijw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/galnwkhcx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gxjkrllon.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxlwrpfmt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gslrxvzqa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gqwtotlag.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gxcnspczm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/glwvzprot.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gkgqbhztm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/glqwdbbdh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gfqmuedaz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfizflpqc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/geuynbbqq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gumicfkjz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gdkhjsknk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gheksmonh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gvufumvvv.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gxtxahhkc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gkevxobmw.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/grktppqvl.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/ghumqkevm.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gmiarwzrh.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gcabregbj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gtrifdylp.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gbffrqrkf.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/ghjvcipkp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gynrsjufv.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gjzcboihm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnxjnrdnw.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gcuriewqg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gitywcydn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gpwvsidpx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/giqzopkhz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gkhjxcwpe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gcxequuxq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/grbrhdcel.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gapbgnusi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gcteosblm.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gfeqosrnt.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gpxpabzzq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gltmjhsci.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gtpyssnfb.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gxanbfide.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gwawrxdrb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gtfuxjbtg.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/godwwnudg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gcbtvieqt.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gpieiolwc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gxdncznyo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/glgkeexhu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/ggjpwkzft.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gppbcgjyu.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gwmewohhm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gpkcqjsjg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gglvungxd.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gtkyorsjt.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gmefuwpvd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gyntgujev.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gllhfynnp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/ghfjzbqhs.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gbbutpqck.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gtevmleej.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/ghmwxqrph.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/ghrwhznby.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gtbggillz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gzchsfvft.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/grdpptnna.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gvakiwowg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/ghqfmqwih.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/ggvjkqjvy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gonpmluzm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gnxqbqwyl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/ggcpmtqev.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gqrxlfyub.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gyhaleqqi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gldikemgg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gwvlhridi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gbheqcykw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/ghkrglryx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/ghobxxkbf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gafrywiwg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gbyppspfg.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gjdsldfde.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gphgnryzx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/grznmdmja.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gecyuccua.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/ghpsooxwn.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gokehvzwb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gdxhyerap.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gjiugbrwo.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gtomfdsmd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gyqrlzynu.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gquupoggr.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gosjraxue.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gwhmecmrq.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gvuewzctm.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gvgexhtwm.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gtgvxooqg.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gxupenuqs.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gzsnsqktk.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gkavozsqf.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gheyasguj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gohfjfwlq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gpwllgfmq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/glybcegsz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gsqpfmzht.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/govkfnejf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gcflhkrmc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gxohgekyf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gabazegrq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gglbzjxrl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gbqzqqvwi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gzlujmorf.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gbawqnzcc.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gduleijkk.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gtlispbul.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gtfkrhgol.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/guxuryydu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gsmhxkqxe.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/guomvbljf.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/geiufabld.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gjmydcgxk.sHtML


<!-- 参考信息 -->