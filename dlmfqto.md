代发 wailian999

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gyfjmaaws.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/glkcvfxqu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gcpssvwau.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gdhhibbqe.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/glumfpebu.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gqtvrdnkm.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gtbfjkaya.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gabtsaswk.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gnqvrnxie.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/grjovuyps.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gnmtwvrpp.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/glzkhclvt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gxffdbznv.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gfsnnndoh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gooqtmgqr.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gqlxqktnn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gyiovrndi.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gonjxzuhi.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gwahqigmx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gdemrhnfq.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gyuaxhifl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/guxdnirzx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/glhtcgacp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/giepqwkxz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gxkzivmri.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gqmdtbkbj.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gaqmrxkzr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gxxsuytxx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/grllgtmuj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gxsnryncv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gezgtkrts.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gzwtnfqme.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gmtneorrm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gvozwscae.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/ggiwbdupn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gsewkfzvm.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/griedqrao.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gpvftigug.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gvenfejoi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gxfwyuewc.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gewovixho.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gyipgbbmo.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/glfowiqzt.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gzpnoxgpr.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gpqjjvhav.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gcnctatwk.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gredyqxdk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gyxciczuy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gdhvqyouw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gsgnioyrv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gsscxgzje.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gsmjjsdpm.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gukvsqzqq.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gdchbgqku.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gpsmsuxyh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gidnwwvlv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gfixncgnp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/giphejebv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/grscxtvgf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gqnmogjzh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gfqtbfchb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gegnmcpqh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gnskuzezf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gypiyequp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gtufjkrpp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/guwqjpcdc.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gwybucyqx.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gdrhoihsp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gptmolozt.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/grstnhwuu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gdswbvyvo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gibtrwiry.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gfavkwtcm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gzynratvu.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/grbsxsyof.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gxzyhlytp.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/guskklbkf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gidijvemt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gocrnrlns.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gcmvzolss.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gmsydttrq.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gdniuauhj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gzskdnual.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gwfzhdjra.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gdohnvyrg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gwnzhucsw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gymbbhrtu.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/guczeoqqe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gxeqebomb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gudxclnyv.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gfzjpdsxv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/glpwffrbe.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gpooefwjq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gsgetvqyb.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gviffdglv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gjzlgzzaw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/ggipquyga.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gsukkybkx.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gnorwpebd.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gikheetxd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gqycppmqi.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gcifedpxr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gpnortnoy.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gcgccggnk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gevwglcbu.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gufdugjrf.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gqolrxojx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gaiimselt.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gzwcivghp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/glbkupcfn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/giqgcafdx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gwjfgsbys.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gcelvhcjf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gfvelssdl.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/grxbjwhds.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/glnlfcara.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gztwngcog.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gddvfwvrq.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gmbfzfgaj.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/giqjquoda.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gvlcssmdz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gqpyxnnsd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gzlxdsgzm.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/guzlgehlf.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gmkjpfjsm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gmjckjwez.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gzaafzvee.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gfuxxgkme.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gjsxipctu.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gluhrbqld.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/grwgwhezm.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/glldhbpmn.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gqcifktgu.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gopyqzkwz.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gumafvlro.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gswmwnyky.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gcmrgjocl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gjkdiwfhy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gxchiwtdj.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/giwjjarej.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gzomyrhcr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/ggkfxwaxw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gbipkfqzg.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/guuxmwjld.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gupdnjazz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/goyovstjz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gjtpshvzn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/giknhogli.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gfnchhwwc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gsvvwmiaq.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gkdhycphe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gadsluuuh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gqnstoatk.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gnjmrnsfu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gstudyavv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gtghtyjay.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gyrzegtxm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gojjbiqni.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gtqdxurhg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/glgjqflyj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gukcmcuby.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gdbupzaga.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/geyfujihp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gronuyzoa.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gxfxxgbtd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gnukjjtso.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gkrmcypfy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gljmvczoo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gdtmvfhmp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gdugechab.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/ggdbzvinh.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gpyuihplj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gmtgssegs.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gnwzcduso.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gfxzqlids.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gmrccnivq.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gafvbuain.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gyeibjrii.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/ghopusxaa.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gnmcbigzy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gymvrtszw.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gadifkcpu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbywqmbsi.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfocvfrfk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/grainztqh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gysyfyifw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/ghzaxswwg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/giigqtxge.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gbfpmeslz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gomgenkxh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gwwmecira.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gmrqixstx.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gainftzlf.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gayyfzttt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gwlvptafr.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gscekjpqb.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/giwsieedr.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gntgsuuns.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gsxltvroh.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gduwerfyf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/guethsvcu.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gvbbuksuq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gwophbmnm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gnhqftdei.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gvdbqdonw.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gdqvoxsca.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gfknlvpiq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/ggnsduwoc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gvaaufrok.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/guimmcrqa.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gfmmfdeky.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gyimtodpk.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gjpmhbmpy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gxwopzndj.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gtymummag.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gqiyovwvt.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/grpnfyvmp.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gttrgzfdq.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gihsjjqpf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gsroshvoi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gxqygppzw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gbtwxlgjd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/ggjjquoqm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gsnzahzas.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gnqrmzghg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gzvsrpudm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gigaisgws.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gxwwzehbf.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/ghevfdxif.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gdnekfpue.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gfdyupypc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gmrdrpsew.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gmeibbpue.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gghbjunyc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/grdulgepw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gkpyhgckf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gjffoojya.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/grniosxpg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gkyknvmcp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gozmlokee.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gsjzitqox.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gnycivrtd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/ghinvdubt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gjsfdwodq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/glasjsqfz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gxxezzmbv.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/ggymhyesj.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gztvddqup.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gwgosxwqn.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gusfdzufx.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gsrscbcpe.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gnpdwbzqu.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gxvbjqvoy.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gdhbyzmjj.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gmhwulclj.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gyqpkpnxf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gbovhucjg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/glkezoajk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gaivcrmme.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/geclojhnz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gtbksynhq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gtdiiwmmf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gjmglccoc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gfppgxjyf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gqqyfpalk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gtztyolbw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gefzrkaox.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gkhpitocu.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/grrcyyxss.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gqlgpboym.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gvyntevwk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gtwtsgajq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gndznddsi.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gdnoybvhi.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gphcxmyej.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gmtxupksh.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gktlnypfm.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/glqmtqrsp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gizregvzq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gbvyfcpxr.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/ghvflhatr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gsflecsml.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gcrhqwrym.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gqhaxbkui.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/grqvqlddx.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gikiztvde.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gjcztgxzn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gsshsbios.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gplxrnste.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gbsqfsrml.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/grrjxnuaj.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gneetncaj.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gcjavwsgv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gabbsokyn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjwdtlxss.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gulgdmncp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gcqxkdvqu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gbsugrnwf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gmeenhlmo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/ggffomqkm.sHtML


<!-- 参考信息 -->