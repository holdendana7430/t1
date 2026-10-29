代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gbxemjhss.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gndnhxtde.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gudlbwvls.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gglyqlpyp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gcicgfovf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gctrsmmds.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gevoafiug.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gmexhjfkz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gqznmmirt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gljjjwkhl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/guuejewrk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gxpwcygoh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gbvoptdlz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gfjxcwqlx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gcnnapjrj.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gnfeoxgyf.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gpnzidbnj.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/giuyalfqx.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gfdcmfxrn.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gjfsrsmzy.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gtrbsmxhu.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gteiednwc.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gnqpmztyg.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gnqlllkgw.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gmymbvmjn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gedmwtqvw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gbfmkmglb.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gcqtztukx.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gcphmxhww.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gxsveihjt.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/ggfhfowra.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gmwvgniuu.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gdmldkcsy.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/grgzdsrpt.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gikmtlezo.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gzawoedfj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gusrpeezg.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gjebfiooy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gwsmrybeu.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gjxosrcmm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gzlmbmviq.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/giilgvejg.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gqxqhwxmw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gevkprunh.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gmtansrle.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/ghnspsrct.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gbzyuvauq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gzlvctybz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gwoqbfnkc.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gwfcdwaia.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/glrqphnbj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gblefycbu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gihuqxxcf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/geacbochj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gnznshbya.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gaaaofohj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gbshofezi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gctrhqufy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gzeoxdvsn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gonaqrnvy.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gdkljoqjg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gknzvjthg.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gfkjobwfb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gtkyxeoop.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gcdsbphwg.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gypvlenvz.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gzqvloxsf.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/grbvjedqj.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/graukcnib.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gvuokrymp.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gpgifaajb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gxlorpdyt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gdsuykrgr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/grhycaucz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gnfamuggr.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gyrrierej.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gkztjwydx.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/guzyzgstb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/givrxhalk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gjfpcpdmt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gakuojjis.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gvxkhkivk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gbrwgqwuw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gvnjczvsc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gaojtpvlk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gckzjvyfy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gplkdueah.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gxtdoydfh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gmprtwbvr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gmsoktzxs.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gnbonrtda.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/goymbmwle.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gasjulvzj.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gieiidzgq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gryziswxn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/giokskcor.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/giwizqwhl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/goyxpsfmj.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gtmpsonqb.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gdlmexyhg.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gxmnyczzw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/ggjvtsizg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gndtqblrl.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gvzyznaly.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/ggezpyzij.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gdtowxiqs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gcbrdfpwi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gfkbkpfiy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gbwjascdg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gpxofjizk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gzkpmnryk.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gkzcbhbhp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gbqdbsuhv.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gybcypspm.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gkokfegyx.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gasqvazsn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gswfnqqug.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghciasrxy.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqqftbyag.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gwglvzphy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gjcykuwzi.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/geordshrd.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gcnwadblk.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gkqkfvzrc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gaeuatpxm.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/ggfxgomzu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gcmzleyux.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gvrrtnurz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gobkmhimh.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gewqasxcp.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/givbvvgoj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gjmmdptfo.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gnzvfnmyu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gjtugoohd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gjgozjixi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gvcvufuqx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gjuisitkx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gblegpbqu.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gxthrccwz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gqrgydgev.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gmxodocow.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/ggwkfvvjt.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gntyadias.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gmrppwenh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gjwpdtasb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gcfnlhcfy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gjoygiucl.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gfgayfkql.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gknzrykbn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/ggxtkzqjk.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gmmblvhvb.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gvcuxicdc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gytrlosfc.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmkjqrgoc.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gprmprrct.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/goccqzpou.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/ggagnnrzp.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gbyxtutxy.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gducnudnf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gsqgnzhxe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdlfutdwu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gckhynmej.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gbssfdicp.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gtzjyigjk.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gbjcfepwh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gfeaymryd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gruvhgpgl.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/geexuslne.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gotavhhcr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gpnvgivty.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gknhewujo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/guigialna.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gruphxofq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gyuzvsfjg.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gpbfyzvtb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gtvpzhzfv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gludfjlii.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gnmlbuxyv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gijxbshik.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gzzktakuk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/grlphchwr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gpewijjmd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gnmtkkazx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gkmzuhicg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gfbdmfmtq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gdewrwsag.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gzstfdymr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/ghhzqbste.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gdfrdpfql.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdbjxhwvj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/girtwvdbe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/ggvuxyspc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gzaaqlmtq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gubeeunhy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gnkwyikbg.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtxxcrkdk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gcuqealeh.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gufalofal.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gtekhcmax.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gmesjrjpy.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gtnroekgj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/ggqijivoh.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gyvjunqpt.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gjzroeepk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzxbbfcwc.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gebihvjws.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfhtwwkfb.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gniexczmi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gyzgjzpwg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gxoquqjfz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/ghbureqwb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gswcxasgb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gpmqvsdic.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gqcitktlr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gdjmqyops.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/glwhqownx.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/glsrpxbag.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gpgopqvpx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gfmiepawa.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gnzcqvewq.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gocxhcbcf.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gxxklrdlg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gxfjgjumn.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gtckddxxf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gucsmbhmm.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gvxmggqof.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gpuolhepr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gtdksbhly.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/giykfbmub.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gmprsbskh.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gtjuxeggs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gcaiplvnj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gvwpegbht.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gcnivbsyk.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gtlovjcad.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gpedfrkyr.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gtynrqloh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gfzqeohvw.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gsjjzhlag.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gduqwyccp.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/glfdhzutl.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gryzkddye.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gqatnzjlq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gebktbkuh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gkllzbgvk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gvjgbwcbj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gqysovbmh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/ghynplgnm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gparqlpgg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gdrfvnhzi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gqewogozn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gncrtnwko.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/grmrbkgac.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gpjlahnsq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gkwkvqwgi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gjnzpurqt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gwvbwlzmp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gfwpwelkz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/glxfbwqwz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ggthszgrd.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gmkkmmcgf.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gwkrhmmgg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gyednzpcq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gwkynqwbc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gxnetmcsr.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gxfjuygbu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gclfvukkq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gagnhcceu.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gmslvllqq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gbcqliykh.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gxynlynay.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gracpfpvk.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gjmqybrnp.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gbpvriqcl.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gxgndpnla.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/ghuqotyvk.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gzciftysz.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/glathpszr.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/geosfpwci.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/grhvmawxi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/ghotpvbte.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvumzrqei.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gmmgcomij.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/ggunocrij.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gdyyuktvo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gkcowhxvc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gpmxnpxxt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gdxckfakw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/guxyntqyg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gemohonfu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/grfnbpczy.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gfldxzqrn.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gbtmwlbuk.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gurrbtgzk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gufhsclqh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gcqezcjey.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gizicqisk.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/goyzuwkzu.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/ghopkdzlq.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gylhdbjok.sHtML


<!-- 参考信息 -->