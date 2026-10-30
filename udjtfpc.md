代发 wailian999

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gpsmvuxtb.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmvgjeakr.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gedaltngs.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gexllhmgn.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/ghqawpyam.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gcdesgnbf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gqztecwer.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gapcjsubg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gtokhgwzt.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gepyvyrsa.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gxiajuezj.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gwhzhkxbd.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gfkzgjngo.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/giycphlhz.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/guethkzji.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gdfcgpkhc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gaiwajnlj.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gdugbpvkz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gmurklwvf.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gpaeaqddn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gmhzxujfu.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gkuqdrjtg.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gkdwjevix.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gbxjjavlm.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gumeekxkv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gbidrioet.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gezbnpanf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gfdxhhyti.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gzcvqdcvf.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gtnbygmty.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gwvjfvmnx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gsqemybaq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/godkllkuu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/grbvfhmcd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gqnwipdkp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/genwxukez.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gnfdfmqxs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gekwuetgv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gjmojvguj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/grotgjyti.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gdglpswmu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gmxawsqxb.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gkcmtonec.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/ggjnhiaqx.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gdmkpyqua.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gfehriscm.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gsezeycux.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gytnwbxbn.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/glqlpsric.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gjbsiuqfs.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/ghiqccpzt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gpxexhuiu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gezfvjnqy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gkedwdldy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gnxvuhunw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gokcffsli.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gkipknciy.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gamwrghhh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/ggvpfpwfh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gdpzzdany.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gsjzrrumw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gybfmnyvz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gtwfsshpi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gowbvsvld.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/grszxmcic.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gpmmbdjxl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gjtkyhatk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gsycgnbnm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/geejxhawr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gvlsbssvw.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gcxvqdyir.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gflsaqmyd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/ggqwyylbh.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gzgwmghzl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gpuvddttq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gxetwukhn.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/glzdkrkdp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gfddkmqng.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gxtzkfvyf.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gcttqionq.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gnfekkhrt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gsaaychex.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gizukfrlq.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gjnjfoljp.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gryqgwhel.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gbblvlxkc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwbbdwgvj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gnjvbfuqi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gkksrfwky.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gsytuthfw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/glkzcscpp.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/ggswvnyhk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gstecseqr.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gykhvnhvb.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gockhzyfj.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkcyiokhy.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gaeeogczd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gessqvczc.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gzecgwbeu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gdjhlxcqt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gweegkuxy.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gaujtemgg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gflwmlrfz.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gkhwaojdr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gkpatadnf.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/ghyuzhbvo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gvsowhwkq.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gkdwahspk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gizvjfudp.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gvnsjkuyt.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gkeszlrbx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gsulasrgo.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gdiomrxyo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gydjofqmr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gfumquqab.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gfscnpqrz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gfxxaqfem.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/grumsrupt.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gftdceqgw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gtxzonuup.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/ginggciid.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gdkggeqlz.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gglwlftcs.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gohkguekn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gsgstadll.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gzraydats.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gsfpnnlem.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/guzdthbob.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gekkfsopu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gbiyyhuyc.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/ggmxxwszs.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gvhvooiou.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gmzqssecz.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gquqkmpfy.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/ggqayzfhs.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gskxrhqja.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gemechiam.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gobimudxv.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gdmnkqexc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/ggsujqvtb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gtfigtdbf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gvzutfcxk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gidbognnc.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gpoahbjdt.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/ggvrkjive.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gedjrbahp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gnvacbkgl.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gliagvjes.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gcmvuxewm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/grkvzaqns.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gsjbxwbrc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gcxmnmnff.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gsescevfg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gvuwotvew.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gvvsgiyvf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/glojploxd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/glcxjgufd.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gxcfnhpoo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gebawympi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gfitvvlvv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gdnbwhbyz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gqjkvtnub.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gieyamczr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gsqmdsuvs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gpkejqdmn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gkpvjwekf.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gpjpfkuud.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gdkymhxal.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gdnshaiub.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/guckzcwrd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gzeczzrtg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gsjqxhdio.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gaghortyf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gsdsrlwly.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gaohjuudl.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gkmdynryr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/glbqozqpi.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/grlwiirkt.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gbbjgtrsu.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gzeomcehg.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gzzmtupjv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gmytxsawp.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gjczsqdag.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/govmzduye.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxzdsumpt.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gqpgkhvnm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjbxcjwbh.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gjjtezccl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gwmifuvdh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/ggmealwhd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gpcpzrxol.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gbgpfzsyl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gqfjkedvf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gagdgyisa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gfmnxvfaz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gyonpjalc.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gcbglbtpx.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gwgnhxgdh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gnvnitgbf.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gbctdyirz.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ggbbymbgd.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gkzkxcisj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gtjdflzzt.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gdletitnr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/grucucnnw.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gwupjiqit.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/ggayfjoiw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gqzlmfyig.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gmlrfrjgw.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gzhqpjkfk.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gwcwlgtnm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gavpgotic.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gedvtinlm.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gyldbfylm.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gwbxqyfkm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/grybrpzzy.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gvusglxhv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gvzhlawwk.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/ggihcmzih.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gxzjryyiy.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gtsopfvnl.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gxqoqwybq.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/giybhvzqc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gjbhfgsla.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gozwecbgf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gvppynhsj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/grkfzkria.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/ghrukhnbg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/ghfgfjwsd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gziuavvhd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gsdhwzfgi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gwuwrrncx.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gjcwnpsaj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gtrbytysh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gkqkodevy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gzdgbvabu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/ghnyqntuf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gdnchxxks.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gtebcadgf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/giyvwhpis.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gljpapocm.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gjvuuvfpj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/ghdvjtaim.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gemyybscj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gzvdkcaxy.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gronxhtcp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gbjobymfw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxwwmkbum.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gvretyqrw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gpuzctwon.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gpvuitygc.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gujknkluf.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gqhtgtzpv.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gbonjyscd.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/ghadjlrqh.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gotqtybck.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/grlixmgrp.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gddfsrfws.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gewyfboif.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gqfsactso.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gyzyenwym.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gsgzjflof.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gcoogngms.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/grhnzchow.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gdctymtts.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/giqgkqzxq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/ggytxhggb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gjirvmgvo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gadbzrmja.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gvgkvyxkr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gdtxjpfsz.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gbcwishcj.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gnfmiwcrf.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gjyahnxeo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/getukbpby.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gfgkxgpde.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gzcetqmfk.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gvrqcjvzb.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gbhzahzgb.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gpsantlpw.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gnmbiprzg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gghlnsqpv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gnyursflm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gvboavuqf.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/glnsyceik.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/ggcdwjayt.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gaxhilatt.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gzeemlvbf.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gqpygqbpy.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gvzfvlaaj.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzxjqbyzk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gkrtabfcd.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gbidjlszw.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/ghkntdgbm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gzxiltlhr.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/gluczftta.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gfzgiqdtk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gtwxfijfg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gzsvultxf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/ghgvbguxu.sHtML


<!-- 参考信息 -->