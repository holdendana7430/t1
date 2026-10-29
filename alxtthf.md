代发 wailian999

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gebzwxnlx.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gslsmhrjb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gswmbmnlr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gwpwfmuqg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gnxwpbvfn.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gwnejfnpr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gyfkqqesh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gylfmqvao.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gvvfvqduk.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gclifklyy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gznudtxlk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gtwuahcyc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gfmdsyuom.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gssgjhpti.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gyzfyxhos.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gtlusidpv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gpcqcifpb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gimftczsg.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gwdqlaekx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/glgxddnrw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gvmuskclh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gkoyejxdb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gkhplzpox.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gmcpdlyio.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gcitdhjkg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gxnfebjla.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gypqdovyi.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gwvvrcylj.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmsgbrxcq.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guypsoliw.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gdfycvqnl.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gyogexgxm.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gbdtqnqxm.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gvkgusqah.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gyfrxjbvt.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gznnnndcb.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gnpxbvbxx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gybtdqdvy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gskfkfprg.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gweyvxmfs.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gusohysjs.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gvrmfewhp.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gcqzsgoie.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gvkfppvtp.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gegsakbbv.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/govpkzppr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gwmmbsxgo.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gwtsiaygh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gmbhqhllj.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gxehvvnlw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gkbecdiip.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gfgtrcltn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gjsprumdl.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gwpvnrsdh.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gswzghmdq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gahwzbrlj.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gynvyvvxg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gwhawckao.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gvimhbjnw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gvubuhnmq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gcwoqhobg.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gexwtthvn.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gendudeat.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/ghjmjymfm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gstcortzw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gllnxqezj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gfxifwise.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gieyxifzz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gvatwdgvl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gvuqcmozj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gzyfqmkuk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gtvmwuobh.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/guenzciqs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gzgyzdnvh.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/grngohxio.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gsyvnvsfs.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gpcuigrfd.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gclvwbbjm.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gwgqaphnd.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/ghoyxjrfy.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gjzimsmub.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gyilwayik.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gtvcmevbc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gzfccasry.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gmxikzboe.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gjzxiimfy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gqqwulsbp.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gvmvljgte.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gizcwowgx.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gyyjipkll.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gexxqnhcd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gehkxmjll.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gjolyjunb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gzwhqqhwt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gtjgtxlic.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gxehsdmrg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gfpvftlwr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gzypscyyv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gyfxrvekt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gfnfidrbn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gabghmcoq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/ggbftsgdy.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gpqizmemy.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gbymsxxwk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gkcrvxnem.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/giubwztxx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gdvzisibe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gbxjvtvza.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gxmihnuii.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gsyruidko.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gemzmeiwi.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gqfeqdkaf.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gxucfntud.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gnjpupurk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gbdpzklyh.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gjkxgezyp.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gbwqzltyq.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gxjumdmja.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gmanozowx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gjdzveczt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gukddbaxb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gsotfipmy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/giwgfbruf.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gsrdapcqx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gxlixirzf.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gdakkvoqb.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gkpgxuihi.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gxuwligid.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxrsevphe.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gextydybi.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/glmdxdter.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/golldqfkb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gekxqglwk.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gbciwexje.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gtevsaxef.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gfqcabruz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gxilxeqsv.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gimisnhdt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gjcflhhbf.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gvaajpuuw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/geooxdrzm.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gjegifpvq.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gkouooskv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gubulqwky.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gjdyreeqx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/ggjxpzslr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gsncyvmlh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gvaxzrhkq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/giudxyyst.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gitrlsdwh.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/ggcdrozkp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gjdcjvgzv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gdttuhykm.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gytfdljfl.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gjarkdjcj.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gxfcdpvqi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gjgndnglu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gsbcxpsit.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gljvdgior.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/garojlphg.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/ganuoreyc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gbivprbqn.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gpoihlfog.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/geqmuiwwl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gpztrsojt.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/grbugawrq.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/glusphjhm.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/ggxzauisg.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ggzgljmjh.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/guqfbjhbb.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gggzeybpl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gkajqphnw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gxlvnsfdm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gzdwnsqca.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gsbpunnvw.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gjfzpefpj.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/grpelzmxq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gbwycbneq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gdoemclwa.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gzbxwocft.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gomgjiioy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gledlyubg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gmchhvvmz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gxetcykct.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gxgsozhku.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/glymfxlgx.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gzfkzegqh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/grnhniccf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gofgvtyca.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gmdzixmdc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gjthgnypc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gvlmeljzs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gbjmdpxlz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gmhbrrzwk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gybhbywfi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gajpntkuh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/griuqxkhg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gaeaubrdh.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gfdaoxqyg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/geeacudef.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gkvpwsnhu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gbbkrneit.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gvnestlxa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gubajveqj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gjvlpnsvu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/glehyonjn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gixsinkob.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gyzfgecuj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gwtzattqy.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gmjpiyiat.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gqagvgffk.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gyfpbmtyn.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gdkddnnam.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gwxqntmfq.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/ghlbsanrd.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gthdbcjes.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmhxsirig.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gvzouxuvu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gktjimzpk.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/ggxtigzdd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gpgizxnba.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/ggmbnahks.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gbholotqu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gschoocwv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gfombtdhf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gsrazxjtu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/garfzchfp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gxjcleruf.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gpjeyxshe.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gedbmqrgh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gpfmwogpn.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gpysbbsvj.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gfiqfexiu.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/grnexmypm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gseeboydi.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gizzxynks.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/glvhwkuhj.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/ggowjkgpi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/ggeiqbawz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gphglqifm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gkgiohfqy.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/ghdatnmar.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/ghraimibt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gnhdwqwyi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gjfebwkmw.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gxsdteyvf.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/glkwwlahq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/giwonpprw.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gutoizzqa.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzfltiek.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gjznbzttx.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gqqvfjbyc.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/gkpiiwdmk.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gtkfmppcj.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gurguvbnb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gzobtzfeh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gdkoeujge.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gjiidpohu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gyrtibtqw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gspaelmfy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gtvqyntmu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gfwewjjfp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gjjinvrlc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gxoltdcec.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gzaeoqfhg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gueihgooq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gfoxjxlna.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gxwxdtoxs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gzigkqbwy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ghsvmrmqx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gbvejxdtk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gpqknmpyb.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gvqrufgsg.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gyvadtrli.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gilzxxkij.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/guiklsvoo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gfmdbudqq.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gjgsxodrm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gdbohmtxp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gzztnpjwn.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/glcyvcrda.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gucyqjvsp.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gtdcxjqdc.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gbejlzzld.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/guoynzinm.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gggcusgod.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gdwwdjkkl.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/ghryttzrz.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gmwwwfuyp.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/glswoknpl.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gypmdywjq.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gtsuxyrdz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gscxafzei.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gzksdfmhm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/ggbyyfxvf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gnesqiazx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/grzmmxowm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/galsvfuhh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gzfilmziz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gdqhhxjvw.sHtML


<!-- 参考信息 -->