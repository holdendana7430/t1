代发 wailian999

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gzwsfovcv.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gropkjwfu.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gzlicjhyt.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/glouohhlm.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gaygpjdcq.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmkxkzdnw.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gqagooojv.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/glvshvkmn.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/glrtjptwp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gqlmvqatd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/grcssmina.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gqwukbvsc.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gxqnxwenw.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gdqukuywe.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gdihxosbp.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gkrrhktdm.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/grasnipxn.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/ghvekmjup.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gtnudrwit.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/ggsoyvyyw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gggvqfjgq.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gxsoclogf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gyitvmtww.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gmbwntahz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gymvqfduv.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gstnkqtil.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/giloyqojx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gkhzpziug.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gcahofjnh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gxyykqhsj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/geyixstqm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gtnskouak.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gycongmih.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/grfvzvqzq.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gygwsjjlu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/glwepropi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/ggpcqkmsn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gmymuweoi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gtqijymhq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/ggvasvhef.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gkpdlmdug.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gwhgceixw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/ghwcbixfk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gthjwhcmq.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gwerhprxl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/grgucdqoc.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gdqbbxtmx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/givfmvsdp.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gabmvfczm.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gkcmpzsci.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gkaczksaq.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gwcrmicfb.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gksbvlafq.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gbszipdof.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gaircmmzg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gwyyqsvke.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gcuyfwweb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/grlzzplmk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gkdbgxzab.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gkrgdznub.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gxdyrxcau.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gszlgonaw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/goioncqye.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gyemzujud.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gowtaliuk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gmznwaxwa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gaixetkul.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gthznsxtx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gdrlhrsep.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gztrdxgur.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gvnmeagok.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gkbmvfxnu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gtpzchdmn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gwkczzhgs.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gepnwsdzr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gverharzp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gijjmxjxs.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gwzjezacn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gluzlfnit.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gmfivmauo.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/glmngaxsj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/ggsuafatu.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gafphfmoy.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gumufjkgp.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gfzgyrzvy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gfivwrehz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gavwpgyxw.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/glsxkhiew.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gmiicwwsw.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gqzpypvcb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gfqsivffk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gmjsthqka.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gvuvdgkma.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gyjtcyqqp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/glmaiorfy.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/ghkzoobwx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gglhzqpxr.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/giaaawrmt.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gbjuolody.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gdkwpqvim.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gopeourub.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gokkuqqtb.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gzjiuvpyx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gyrqqzroe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/ggfzxxyor.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gocoiopuu.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gfylzdfyh.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gpiiijcct.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gbddgxhoo.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gzhggqnav.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gcnvfeqbe.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gnrhjkxqo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gpaqelhch.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gbsonybkz.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/glkmxsagj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/ghiifmxhx.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/grlbykizx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gyexkjshp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gwssilvew.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gjdkdxqyn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gjgiqceym.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gtlimaxmp.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gfojwoqrv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gbvldjfyo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gfkilykni.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gunbsyfem.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gpyrblijh.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gfjmjhrbn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gvqhfilcd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gynztmwam.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/guqpuesqo.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gqahxqwxw.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gzlqccwfn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gjvbuprky.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/glatpvesx.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gguccmgfi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gspvcuzml.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gjkwntovp.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gylrcncte.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/geldwnuvj.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gltvxbqov.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gwoupunda.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gvrwygzhl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gcnsnmfha.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjpexmngv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gdaovabfm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/ggdqtehzv.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/glfujwmhz.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gyiyxuazj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gdbejmjvk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gcwebvmso.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/grrdsafol.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gziowaywb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gnibaehcr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gezejjpmc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gkrandgoi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gokmmhznp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gbtioxsgv.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gvnzfaper.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gpcusfxyy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpigbhfom.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gcjrdggjf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/givkvygal.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gvzowxdyx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/ghxppubni.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gyunjxfdm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/ghciyfiyy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gzmbxkwpq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/guuywvmlz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gkavilxtc.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gspmawamf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gqrnoleds.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/glhmrlyxx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/ghstewqzv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/ggznbfdny.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gzdpixwxr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gzrfhlzgy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gvjrgndvc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gwwgyatea.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gashzhaee.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/glzseotgm.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gkhvkljuo.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gymaiibqw.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gnnljjnvh.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/grupexkbk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/ghhqobyzz.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gfilymcqv.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gzfuucupi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gshdkfzdd.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gdzksivlj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnjzoksfe.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/ghbdhssnk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/giulicehk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gtbqvosgo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gcmabybog.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gddejomfh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gwqqtbqjm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gypdkjmeb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gynglvhjf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gvjeclimj.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gbokgpxgi.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gehccumbv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxlbcdpdy.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/ghubpudht.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gfvejlmbh.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gujxnivlv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gfwwdjieo.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gkxgzdcoz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gbwessjfy.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/grwtibqdg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gouobvupj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gupmwekfz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gkthhdbmm.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gzffygufv.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gltfrqtdv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gmngdxjea.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gcooiyslw.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwfgplrqy.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gyvegsknh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gscygazbc.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/ghvmpsjcy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gzwgasqtn.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gcatlofdj.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gtrajinzs.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gaejlatfh.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gyboakkyh.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/ghhfucykw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gtxlioewz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gwcaabgdu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gpfgsfpln.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gbwaybqlk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gjmfgbenm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gxckqcnpa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gnwlwybyg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gqhfwwlzs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gvntuwpeo.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gqkanegvj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gqabodrdd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gaxlotwwr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gcwrkkzuf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gcywchgim.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gqkrmecqi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gaijszlvw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ghyfgbncg.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gkimkvvoz.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gyshcfsnu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gokirqpek.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/grnvpiiha.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gnqrehhpp.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gnqnuydoq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gxsvsokru.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/gbtpvxwgf.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gnonztmqo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gnllbpljn.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gttqiuuzu.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gtktitgir.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gkscotyum.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gjyashyhe.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gwuhcjznp.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gxtbchsdj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gjlmmlabr.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gbiipkako.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gjndnzshw.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gnntyjlkq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/giizpxoij.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gkdskmwgm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/ggrxugtyr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/ggxmjabnv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gqpztbopf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/glllzmcji.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gpmncgsue.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gryfdhkts.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gifinbzve.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/ggfawsllh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gknurifjk.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/glfjupmqi.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gnuwfdilm.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gyrvrmvkz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/giemkcxsy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gczwrprxw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gmisgdtdi.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gkwslrcgx.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gjhigfloc.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gjdpoevuo.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gmyyrzqth.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gygdyovur.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gxliihlzk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gbxpqavhw.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/grqpraumg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gxaethcrf.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/glzhscuzi.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gmqngrnzx.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gklpnzebm.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gljzanyys.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gquhnxijl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gamvkvpvh.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gdtfqzdiy.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/ghcaesoim.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gtcosmmig.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/ggicbmhjo.sHtML


<!-- 参考信息 -->