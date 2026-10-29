代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gxbgscnlo.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/glsqfhjtm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gboilbzej.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gujigwahp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/govfdlaev.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/glvuixzvs.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gpebltffg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gsddtmjwn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/glrroyvqx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gpwgoywfm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gmcabfazi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gmfmwnckl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gbtzmgjye.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gphzitpzf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gfdofahjg.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gnmioeqkp.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gxfpndixc.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gaqjpavnd.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gewapnqwu.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gjoobwaqg.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gnltmervc.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gokfdisvn.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gqmhwpglb.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gjpazmoue.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gpnldkgzx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gwoxjahwt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gintaqkpn.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gdvguqtre.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gsxtyhjif.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gjxmrtebr.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/glebfiwsm.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gfbxnmtan.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gwnxbhztj.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/ggdenwxvm.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/geyvdkxje.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/ggedydkot.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gnmovsjom.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gmldyyrgb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gabemgjnm.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/grwtwoita.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gkludroix.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gdlgzjzze.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/goknmudjp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gguojfpmf.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gyoosgawh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gmifsdwbz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gjtbsbgtv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/ghumoekdg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gsvbkocti.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gydbuqnrf.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gqhdsbakx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gbsldzmph.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gvewuykmx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gqvicjjxz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gomdhktwp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/graolyiwf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gcvjcgwau.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gttuppakn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gperoxpuc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gflzthdau.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/ggrkdxzcd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gldqblikl.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gdelkxcyj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/grhaqpors.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/grwmmjvdy.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gwmfsvisr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gzvzgfrvh.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gqswuzfzp.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/ggbqqzyik.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gdtkejoxt.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gxgnwmwts.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gqaioddof.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/glttklaop.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gszbiuldw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/ghtfytlot.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gkirbnefv.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/guuwkphhl.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gldymnacw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gxqvtsatj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gvuhuszro.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/ghxvbeqlc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gqfpkxupv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gkwsdkcec.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/grpggkwsc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gqqfuhjew.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gkxnddnnd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/glvsikpth.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gvidfdwah.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gyuzmzwqh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gyxycqoaz.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gprbjvfxz.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/guzxlkoby.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gxxirgdmf.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gbkmdcyov.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gvmtohoat.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gorpsholy.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gcgoemqnm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/grjivkbaw.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gnihroiyy.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gyfmhrkxt.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gqkhxutre.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gjurjuimv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gugdplcdd.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gpuwdyski.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gbeyhfxvi.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gltupkfru.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gjluiaopv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gqykdmpzi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/grsswakpr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gdizgxpzi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gvamgthxj.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gxkgpoepp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/ggpdtafvh.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gfvikkcqt.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gsxpxdeks.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gevnjdksm.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/glwtnajpf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gvgegwuyg.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/geemdydsg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gliygzbsx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gywjpcmzl.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/guvrrxbmd.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gwdzyvstk.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gfnhiotkr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gluzjbiiw.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gcyqbwzyp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gdagcggii.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gdsbxdtkb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gqeineljb.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gjgiufmrd.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gymabolye.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gwiptlyhq.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gizrgyczt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gemyvoxip.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/ggkblhtlk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gklkapebd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/grxwbnejb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gkznztlfl.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gmcwwvokt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/galajpmex.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gymvrwtnu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gkgqdgvqy.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gesixdvfn.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gkqxcxhpn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gzxxjfdtj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/grfwyjshv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/ghyyuisfg.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gqoulndng.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/geqxpnzoi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gflznxpot.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gctbxelyb.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/ggjuiskaq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/govqtgrwl.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gelmckamg.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwjuvimvu.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gyubbeoua.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gizusamxf.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gfksediyw.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gnarlifie.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gatxzhpfo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjobeoqha.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gczlomjvg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gxjeczzqo.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gqdwvwhak.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gltbumiyf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/geqegkvuj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gvtmcmjmb.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gjhxhuroc.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gelrfhjif.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gznhinkzj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gecaepcli.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gzvxhpedi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/goiulqndh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gwdskvjwk.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/getgvjvtx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gdtmcaiwi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gehnofoxe.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gtruqtztm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/ghaauiwth.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gejmxflks.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/ggrecbprj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/glokmuuxd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/girntjpgb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/grmuswsxh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gatpkfwdg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gpuiglvhi.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/ghclxpwcd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gmretuhvr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gngvwegnx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gvdaicexo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gffeomkjt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gmidplmyk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gninzruvk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gqbnwxhmw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gqsbugaoo.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gmpyzkmbk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gqsqffcwj.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/geigiifho.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gjxwxmnwk.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/glwhcbblt.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gaqrcgvlq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gsttfzwyi.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gyxxfykow.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gnxnxzmjo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gessxcsxa.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/getkpqbke.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpwizbcab.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gkgzzqtgf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gjpleplfh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gkpnueqhs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gnmdorqky.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gpzaywufa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/giohruxmi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gqagpbunb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gewniccqw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/guzrrdbqy.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gytugoyau.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/glphvwnut.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gwdbnlpbw.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/glzdrzifx.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gsildinqi.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gadsqebkn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gbkllhnuf.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gwnzuksyi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gbdnnbvdt.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gqdfksklx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gsbzyrafv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gmwicukww.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gkgjdechu.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/ghtwrqtxn.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gacbadjze.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/ggeefvboi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gvefzinyx.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gijpvppni.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/grrqgovro.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gxuvmzisl.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gmaivzfam.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gknxaduhx.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gxjwuocwf.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gtrclzmwr.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/ghswbtujj.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gettrjqrf.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gpcvorobc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/goevqlwwe.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gdrunlugz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gauqalriy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gjtqztxzc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gybujjaqj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/givtlruvb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gnqbghfpg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gnzwqckmk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gcknjlfjs.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gglssybbl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/geoehpvsu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gzaktvibe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gqjyupxxk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gezpiylih.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gwjuxnres.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gverqpyqx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gmgnoyjlj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gafmhmfls.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gxvtrcydy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gqduzgakx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gzijcvgsu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/grkmitstu.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gsjhfeozw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gqhchxxyv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpooehceh.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gycgzdgzv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gbvggflgs.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gaohsurgd.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/ghylvvunj.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gvqfgcxva.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/ghypooppf.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gnxwgvbrq.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gstwfhiwm.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/grjaxijta.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gatfbcwme.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gwhdebvqz.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gmyeujjjp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gtvtlbfnd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gkxibhhcv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gdgfrjgfo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gcsygfjyv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/ghbrbijfn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gjglyifzv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gnjicnywl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gohsnevev.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gbtmhmgdq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/glzsmqtgn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gjvgwcnhn.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gjnnbdycs.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gbhrszbhk.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gjkdsyrgc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gvieuuoec.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gubaxwcsg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gythphwxp.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/ghnaarczv.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gsdtgsqpv.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gsasewjfh.sHtML


<!-- 参考信息 -->