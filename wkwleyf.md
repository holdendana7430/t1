代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gsycqtlen.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gyodpctai.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gskihqrsu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gaciymwup.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gssknizrk.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gtgagkrqy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gtejembik.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gqobzkxpg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/geawgfupt.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/ghyfncqlr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gyogfyhgr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gtqspxphf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gslzgksci.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gchwyseji.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gatjtoqfe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gdbwmvvvx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gwvigqcug.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gmvhaisfn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/ggblmedjm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gjhlurpry.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gniuycvbp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/ggwkamhge.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gyaeoflfu.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gvfciaoin.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gyrryfcwn.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/grofyhxkp.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/ggozqabgo.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gzprfruth.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gmfbufcju.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gzsfmyjsv.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gqbnhixce.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gzvyplbaa.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gzdcufhzi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/guhbupxkq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gbmsbogek.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwhwlotry.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gqgdaauvk.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gapmqefac.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gcuqawtiq.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gmnkrrznj.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gqdcdhlyz.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gtdybkajc.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gbwaiidhm.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gmyzsatdm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gzosrkpgx.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/ggyrsbvpq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gzslsdwry.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gerppbeok.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gzcparakr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gzkyqhnio.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gnhhfijvc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/goumphjzc.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/ghhlvigbq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gmwpfwgfb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gjiqtjbpx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gquevhwfb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gadvapctx.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gvdkwmpmr.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gqigdytkw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/geggtpmdr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gwrwuwitv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gefrbviyj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gvntyxogn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/giwgfxoab.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gswxqfhni.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/ggxyvtgee.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/grmashsas.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gbfzeefcw.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gdcavhnkb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gdsyfddio.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggmqcawkb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/goxoixxjq.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/grpvnaolu.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gjotqudxu.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gkodlylyt.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gfbbgpuuf.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gqawskvbl.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gvcmckkna.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gwtegxnbo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/ghcamrchq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gnbdobrlx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gadpxlbsc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gsopmpujv.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/grooccxxt.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gcypxcdbs.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gwiaknost.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gcatrdixr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gjrkxizdm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gsqgohzpf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gvytspqph.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gnwbnxplh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gibsymadp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gmhobpjmq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gehjtnkmc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gpkodatii.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gwhprothz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/ggdazqexk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gggngssac.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gwbvgyzrn.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/glxdjytxq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gzfbwxvbn.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gwpkcxnoc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gfmgdgyqf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gikqvllcf.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gadoeikrk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/glneavgcd.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/ggvhakfqz.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gmicosruw.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/glziwychc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gayqirkmi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gxznnujba.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gunhhsadp.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gihvgykxa.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/glmppqzpz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gehtwrhym.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gealjudvc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gjigmcrsp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gccahzwah.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/ggwxukcev.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gkgbtetrn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gtrgalubw.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gwivnhclf.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gldnlrmvp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gmkfhkrxu.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gemnkhwrs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gnfhfplne.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghvsxqrok.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gvpnluphx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gojqhzzrc.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gughthius.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gljmydtdp.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gilcfwkim.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gxvrkwmsy.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/grszulcca.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gesickxav.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gwaascpxh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gltufyzyq.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gqnrucnjs.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gtukkaqsx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gfuoahtwe.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gglyyoquf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/ggegbrcrg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/grahgwptz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gpcsdxveh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/ghdlfvhzj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gnszldgpt.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/glpdxiggs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/goxsbokal.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gxyuxtahw.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gfxpdazkl.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gggwhlwoh.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/graqutrfd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gnzfvwyzs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gltawbpxn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gslqivood.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gwjmznxkf.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gcbyfohxp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gptynoian.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gbuvmtlrs.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gmfllkexd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gfyftfypi.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gmogieuxb.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gtgaqbvfw.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/giwqxagqy.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gcdxccnrr.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/ggwhvdqyb.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/geffrtvli.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gbrbzozhf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gryhyjqjv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gsseiduan.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gmuiubpsz.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gaotjluww.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/geyzkroeg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gtdfqraum.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gzynylchz.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gbeyxhwfx.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gskdjncda.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/glsvzbzih.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gnawdavsg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gpyqeypdd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/ggrnrxpyl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gdboseesl.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gylkndobg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gmgtwthst.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gmuzctncj.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/grlqfefuj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/ggyktdnlb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gvffcuwwq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gjxhxucuj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gcokioawy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gfnadjars.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gslucgwzd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gycylfhek.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gwpoocngx.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/grgxfagxr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/guiamxtug.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gjdarfcpi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gdeehxkxq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gcggvmpsa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gjnxazbbw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gycxykrts.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gaolxemdb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gmlxdzpbc.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gkkvjlrvz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gtwmgqyqn.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gkyqobfvf.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gfpsxkwiq.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gxxoplowd.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/grfazehvk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gstlvuicc.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gmdtldcdz.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gmpyghbwa.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfmvhmtgb.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gacebdrfn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdthhlclo.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gnqxsssze.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gwkfzkrae.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/ggpdwicyx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gftvlcvpj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gsiokhlxu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gagdebkfw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gsukmvlhj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gmqqofjxm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gbndczvui.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/ggdxmjxgq.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gjecmpajh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gvvwimzkz.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gpfsuyayd.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gxdzzkood.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gkndbhffb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gsjwxddzz.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gqzmqwvrm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gvboodzzw.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gmodnudtw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gxgtaakgb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/ghodftyzf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gmjtzhdku.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gephzmbed.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/ggygzouwa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gejypdnvu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gaagygdzd.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gpmpxuuyl.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/ghyfytthy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gvwglhrsp.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gqdjtmlmj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gvhdhgctg.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gnzhjgpdm.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gcflafsmk.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gxuoryuyr.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gmejtaatm.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gpxasjuyl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gtqhdnphr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gelyqfuep.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/ghijhvhgq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gqrvfwwkc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gxbypnffw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gkfkaryoi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/ghpiekkle.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gynjojpiv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/grcbakyaw.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gflarbuff.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gbmxtwvym.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/ghmjivpkl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/grorkdzgo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/griklitet.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gifrccdyo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gilyvzajk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gctdodovz.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gnbfidynv.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gyvaspams.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/ghbgbhsox.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gigrxkfaa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gbsqllnmo.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gjcspezhy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/guqkqshyp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gczgucvtb.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gfpmhwdcn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gezzjkmyp.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gisgvvesx.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gmpqwpwww.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gjrablada.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/goimxvqyx.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gejrsffox.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/ghdwhwlxk.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gmmbwspfe.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gzyyamxoj.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gaqldtcde.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/ggssqkzte.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gzuqkfjzt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gdjpvrwga.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gyyhrkulo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gyyhefsns.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gfovlcwqm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gtthfygvo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gvlwliuxw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gghelqraf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/grmeitqer.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gbrrslnjj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/grabvctye.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/giddmnhcl.sHtML


<!-- 参考信息 -->