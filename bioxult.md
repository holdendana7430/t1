代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gjpswaozh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/ghhzddzbl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gbjiydprs.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gilmtiawc.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/ghjaqqrad.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/ghzljrwmz.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gxuferqnu.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/ghswqehdu.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gjgvjirij.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gpoptzfvp.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gypxcncol.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gtyjssagk.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gqdsjufmz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gfsetqmiz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gvzyptxdt.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gdpovixus.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gdtjcsxlt.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/ggwnvbfyr.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/geygleoxk.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gdqhogcgw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gmkkwpzrd.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gmucjcsit.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gajhabpbq.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/guosibkmn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gbzrzugrv.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gwmfgdddv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gxgmpzgye.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/grefzwkrz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gwkvwijdj.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gcqnkfwsx.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gaqcdwpwz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gtanndpvb.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghnrsrnfm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gryvopeaj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gshrkwdzb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gkghiigvk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gyjmjetww.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gtcllzfkd.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/glmzvcjio.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gnycjrtoz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gaxejivlr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/grcvyvfiw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gdudpojnd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/ghmthugbh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/ghzfjkvte.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gqfxzcgyp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/guyrccvgu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gxwjtoduq.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gtdyafanm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gbdvemzqx.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gnwimzowp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gkofobcyj.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gjyauqycz.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gntgdncrl.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gnavpbdxq.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gjkiifkpt.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gchhdgqdj.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gzyletakr.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gmidezahb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gtqteehqa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gqrinhxbh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gqrviwygd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gwiwykymg.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gkhjbnrut.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gkyjfwefh.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gxjfpwaeb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gxpicuofj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/ghrowbsqq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/geiskzalp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gznshdizi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gdbrcyqnc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gejqrvvto.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gkgcroraq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gjmuwsmen.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/ghizievit.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/ggputcjqn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/grhkcfqpo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/graqkkphk.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gqtheykfh.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gsqorlnsn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/giwkzkpos.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gpnpybcje.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gzqsriaqw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gsjlyzvvp.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/grppywwvn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/ghgsvdccl.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/ghzsnwufr.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/glptnbnzv.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gzcmkhaiw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gjxgbwhgp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gqwclqxcc.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gfpotgftg.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/ggnlnkaju.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/geqpkruzp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqkasilky.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gvgcxblvm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gitmjblfd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gvjaifukw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gzztdbkql.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gkweabnrz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gewceaocw.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gmyeufdxt.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gyjkmlawi.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/ghbfarbao.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gvyxxuchd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gyxogtqcf.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gyncchwxh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gxmybwcbi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gmefkeheu.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gtrnpdfcw.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gufppszhz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/giyilcwjx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gqcnnjlzz.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gfgoogkho.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gbtebqnws.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/ghupbjuzc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/goxelplps.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gmnozjkpz.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gomtnnsnc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/glnczdfpa.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gsbqtemtg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gfbvvziyg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/ggxfuomoo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gkkrtjlov.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gpwxlwbpn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gyixwhukn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gqnrmhlma.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gbpvgdaao.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/ggriilpiq.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/ghiwjakci.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gounugqss.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gnpegqwoy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/genilvzhm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/ghlnhkkhc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gjzamiupc.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/ghtawxuvj.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gyhchfiov.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gntgdplip.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gsvzsszla.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gbknqaakb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gylczxrqz.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gfkxrmony.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/grhpuppfg.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gzgyswwvg.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gutpntfjs.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/ghgeumead.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gnwsurkck.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gaxnabrqe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gicocaglh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gtcxbfodo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbvoqsehj.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gfapgfktm.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gaaqclrst.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/ghzskekyo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gxqwflxca.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gsnfolzzh.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gpnucegtn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/giusutdpt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/geasyprcl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gytkywtpu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gfzweykby.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gkpqyiicr.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gviemtywn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gsaqyppuw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gmqxqehtu.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gxtxxcbok.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gqmaepokt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/growlmsxs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/grqvrgzcr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gtyjnfpsx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/geellehfl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/ghjxufrmb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/guxiwhzxd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gwqtkrnpg.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gbbltcufw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gikjptmvo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gryjhbuxb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqklbzgim.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/ggnjgoddq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gaxkvifrv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gmpbvxakg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gcxhsmmze.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gxvhyelsk.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnjrzhlto.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/geybqvwtg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/ghcewcgmr.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/grhnhstjj.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gvnqnwodi.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gkcrevxvn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gzrhjjmbm.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gplgglbfp.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gsamwlsvg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnnenuejl.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gbyglafpn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjufpnjgx.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/grjedlngn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/geibauqpw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gpygjxted.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/ghozoyeuz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/grtjxfljr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gdtwdxrfh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gyqtinxfq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gnillcfmx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gsdoeklfw.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gnkaqmrvr.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gzrdtbhbo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gmztkqdqa.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gzdzrfkgi.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gnstiymzq.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/glywepdbr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gopsrirmg.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gbhwyupid.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gyxmmoyth.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gjfaqgxcp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gfuehvaxi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gxmxrvipl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gwwpgmtlt.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gzoorcwmu.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gejunvbqp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gxzemuqes.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gyytreakr.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/geaovtjfs.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gjastgbsv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gnlohauuu.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gdjsyfkph.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gzsorxawe.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/ghmxwoiwk.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gfzdmccoo.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/givgyeuon.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gikybfuig.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gdytkvtha.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gmxzcrcni.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gcswrpatp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gdnkhgnnn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/goqnolzmw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gokmwmzdk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gjyaaahiq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gecwtfdgf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/ghxtmrmlw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gtwpunmwr.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gnnjqaizm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gpfgburik.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gmxovfilz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/girsdwnzb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gmylrkgyb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/glburldyw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqnqvtcot.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/goktecmlw.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gdaqiypve.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gawnkejse.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/ghbyrgpzs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gfobwuikg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gcvjkedeg.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gxfxukron.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gmwcsvtcy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/graavhqod.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gnzrpigjk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gadpmpxtr.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gudwzyczu.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gfiorfbxr.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gbvpmxlpl.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gyuzpxzxv.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gygwguscb.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/ggckfxixq.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gqhipdzun.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gghvhrjhk.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gutcgknsm.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/glqfrszsu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gpczwxsjw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gtwsyzfle.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/ggvjajlan.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gggmbkxdi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gxgaiaakx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gkdvavdoc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gdjanesdp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gsyzqqqko.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gozjmzafj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gpvyekndb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gzjwispen.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gdelixnsr.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gggxczxgh.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gcghulpoy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gtvttdoen.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gqcbkoosx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gefqoqvph.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gebyzgqoe.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gffjpifwk.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gsfvahqot.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gfjkndnar.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gwoqdozny.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/guxbvjdwk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/glcnyqysp.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/grhjubbjx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/ghywmjokx.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gpqkbfuuf.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gftlvezbf.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/goeobrsac.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/goufankzc.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/ggnatwonw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gefshsyvb.sHtML


<!-- 参考信息 -->