代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gbeqfpiey.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gpbipepdb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gjswfaqot.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gnjssfjum.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gfchhgfjj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gydfqrblf.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gkyauefwi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gqmdqoglm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gucpamtsb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gvnlnzksw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gbueczdhc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gsfzmopku.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gmymmfklu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gxoxqlibu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gfskssibl.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/guwojevsz.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjlwjwuig.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggjuczyqg.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gofdwtbbc.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gveduxysv.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gfqopogxp.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gahwbhlvp.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gttdqrkhr.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gurhiugsp.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/ggubnzpxc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gifnazddj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gsupfcxsf.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/glaufjghr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gyckwjumd.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gmzdotbbq.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/ghplpiucd.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/grzlnbbjd.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gsxkyspuf.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gbpasmlyu.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/glatlsuvk.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gwkpjzkve.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/ghzcdfpzn.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gufkbpgfh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gjapeinvp.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gbmpqdswc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gyhxkfjar.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/glzbscnxv.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gllgfcolu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/grgntxaye.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/glxhrfdyv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gkvbelmey.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gplfzfcqm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gaohzvhqa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gsdttfwxm.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/ghhzvvehv.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gelhifiiq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gcdmldcuh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gsxgdmkzi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gkxwfojoa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/ghewytcii.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gnitiznwj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/giwsfiwqn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/giisiduvq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gznzydilc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gwdluhyqj.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/ggtnthgfr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gylpvaumb.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/glfnsebxa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gzxuqprsy.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gsmuyvvup.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gvfmfgajp.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gksovlwhd.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gatolbbpf.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gtsrtcjsc.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gsmaotkkk.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gjgdlzgkm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gnxewxick.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gfdaqifqo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/glhkhqarw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gygbyfrzi.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/goalddvpp.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gisyletjy.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gabxqklhl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gmzcpodxy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gzymcgafv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gzannfvuj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gffgmrsjd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/ghphyxfgv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gphcmcode.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gvtlbwpaj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gavblbcmw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gpggvyfst.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gndlzcyue.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gpclnsllr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gejcckpyb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gdlqmynej.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gsmxrkkbh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gfufjwwgv.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gxhjhojvg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gcwdlblbc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gawkuokae.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/ghbhvapky.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gyopbscvi.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gbphcbuce.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gkcmtdnit.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gpuyckirq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/guqnaxvhg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/goxvdupza.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/givwlunip.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gpnrerioq.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gctposjcr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gehznlckq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gstivjtnj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/grmbsdbvf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gbqcnijsb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gzumeieay.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gvqafsttt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gnvpyyhzw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gladkcyfb.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gyvbctehl.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjkhvshzk.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gkslegctu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjhxwowgd.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gnrrwtfwh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gtfcgpvrg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gsrwoquql.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gdfyvcdtf.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gnktokdbr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gxwkrnwxq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gxowgfaog.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gsgtwwdar.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gbonuirjl.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gedpqpoub.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/ggipdyzoo.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gmrbflfln.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gxrisomkx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gbavtsghb.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gbnzxqwrr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gnvewhqts.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gxmmupekg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gwjofrwax.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gqqcxysic.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gfrolwzjw.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gzghinsjh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/giqulqalg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/giidzbxfu.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/glgpjlkav.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/garhlibni.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gzoysywwl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gykrjcuyl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/ghtnbgffg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/ghyeekqcx.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/geowupvsy.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/geklmhhoy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gteckmrdv.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gzgcjdkuo.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gwpaugapu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gjqfizlxr.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gvjsbopyx.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqreoelng.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gbrlkketf.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gvtblarae.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gciiyuuao.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gwicmfkok.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gxohfljge.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gfsjbocsy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gjrguevsl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gcocbosku.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gnlfseqwg.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gvlgaaloe.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gjhhrwjrx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gyvhyrmsd.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gmfvefxja.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gwuatnzzh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gdgjqjqjq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gloksducc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/ggjveirii.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gyabdyykm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gzagyeruh.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/guoadrtrp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gjdjirzbi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gmkkiqbnq.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gfclzgtln.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gdpushwww.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gpbwgfjdz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gomurpkde.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gajjuddun.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/goqyeykrn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/ghflmtblo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gtbzlkjvc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gqfeqazwe.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gflxbdbcw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gbtcrximf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/ghsrwatib.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gcoayzitz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/ghxxvgrxp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gmaqqwqzp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/goyfrataw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gloznqmgx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gpczrhvbq.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gqixhhmub.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gakslxshc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsppamiab.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/grxedbptb.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gqmlsbeew.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gegivrhzz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gkodymiwi.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gwnfbwruw.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gootneowz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goynjrupv.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/glgetuwok.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdkrfcfon.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gybjzkeha.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gzuiwzjsi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gxhyrbkhz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gyrudlgqe.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gncdzcfgj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/ggxqiciad.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gumnkkowm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gxhdugrlq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gsnuktomq.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gskombpqz.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gxrcecuqt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gypytoijo.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gffmpkqvv.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gfxythpxg.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gbzqfylwv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gueljweap.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gsggicodp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gvdhvhzmr.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gflglyjjy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gohkknkrk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gvfeyxgur.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/grmswfxub.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gcbblwncl.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gzchbxqad.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gijtsmche.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gtznwbdwk.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gzlkmlazk.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/ggwwackfz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gcptomuft.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gcnzneods.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gpjvalgjq.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/giverhfgv.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gamxnyhfs.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gtznlmill.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gvaqgplvx.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gqjblmpsx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gjxydxzmv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/glbfptymr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gluhchmbn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/ggbjnmwco.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/grhppmchg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gmrvmjofc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/glcxpiynf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gxpeusatk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gmzzwyueu.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/glevymvqf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gtergmxji.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gsfzuunts.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gsmmccloe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gmuqqjzpy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gibkbstkv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gwozsmibz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gjnihkdav.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gnxjqnfbl.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gnnmpvpgn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gzpgsgehz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/ghqpmzoiu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gopdwdimf.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gauxqjufr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gpmzeseot.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/grjazomad.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gqdzbxppt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gfpcbubee.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/griygsiey.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gtbaxaiuh.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gwoaoetnd.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gmqvpgrup.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gzzmpncti.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/ggrufntyh.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gpynjjlut.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gcjlfhena.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gfqjiarme.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gjduqtxte.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gvsfljqoi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gfgmafvnw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gqanailme.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gforjcqxj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gynpsihbg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gpxrksyvb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gjomuphtw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gspoxqhfp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gsygdbqpf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gbfrjurma.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gucjrscfe.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/ggrfezpxl.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gmwfuqwlb.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gpygvkhsq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gtbnzyanb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gghvqmfjp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gounvwirz.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gmfpicqfw.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gmmjabhum.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gnifferjz.sHtML


<!-- 参考信息 -->