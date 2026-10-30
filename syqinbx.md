代发 wailian999

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/ggkpfjjni.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gssyoygvt.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/ggmnlsrrw.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gigwbqdux.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gzjywajkp.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfhsspcfe.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gsyqebeyt.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gqcvzkbsh.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gitzygfkd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/goizdggfb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/goegjasez.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gzrekntyj.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gpbthvsux.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gqjmyxhoq.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gnpyxwtwz.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gbexzqpeg.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gossgkuzp.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gzzdlunuw.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gengypqnu.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gmranjtob.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gmtmbjacy.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gugidevfk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/goswewyil.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gviqpbdyc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gyufsphhl.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gjdkevpxr.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gijcblwqv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/ggukrvqjh.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/grxxuaply.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/guimqwivb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gepztuqgb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/glunwdrdn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gaafdgaip.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gbuhqhyfq.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gpwbsikpm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/grziezpql.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gyqipbxsd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/golwygggg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gfhdtiqoq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gxksubibp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/guprwqxgn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gjsxygeet.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gsogarmph.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gzgpenmcp.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/ganfylbdc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/giafzuqdj.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gktbymijx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gzfphpmmz.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gdzhgodke.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gxdburxmy.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gqyyvlqej.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gbwwjpykx.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gliebiyaq.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gqvqdthes.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gfmmoytrk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gnpkdsfnr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gmmiyqquc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gmqqgkkps.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/geehfbkfc.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gpihbrpsj.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gwcvpiuhr.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gqsenuajj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gvwuxnini.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gstwxreeu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gpopktjaa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gmkrcyotd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gqbytvjns.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gfqhxxtep.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gatnxkcfc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gkuxirldq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gqujfsygw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gjgapdbpg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/ghgfjhueu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghccfxewc.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gzrrglpwv.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gdbbiccsx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/ghrctgzis.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gsomjipby.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/godxwgosu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gftbmvjua.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gmqjsykup.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gonztqjmj.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/grtjcmegw.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gvfbgqhse.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gauugrlco.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gdbywxfkd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gcvnjrtsl.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/ggbtugsul.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gokbchefc.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gtqgrbprk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/giteijari.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/globgejme.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/guhyterdo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gufayhxjx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gmyxijvlr.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gqltmdcaa.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gazpgrliz.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/giksdjhuj.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gvoscitzu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gndqqonxa.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gsjrezniw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gytukunsx.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gzomgstqv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gpanjcgzm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gdeaahjrz.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gyqccqqml.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gsfmoeulw.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gkpismorj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gjhjqjxvq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gptvfaenm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gmjwvmabl.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gyvykgmpo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/giueacxoe.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/glqixdtmc.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gevdwpihj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/grgdpctzw.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gryjevdyh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/grzrsfvas.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gkeybhxos.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gzeejrtqh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gtpfcyqyh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gnavahsiq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gtubrwxqe.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/grxvsnfsc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/guqvsybcs.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gnqvugomj.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtjwymgqk.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/ggrcntmxz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gttcsbgyn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gktndhihy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gitybsuyo.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/ggjcaswmh.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gfhpbtdcm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gszwicbvl.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gebwdxvog.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gnzldifvg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gluirjoxx.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gchzneyxt.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gescvljki.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gyjgcjxxa.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gaforzzrh.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gtpjchtni.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gfybakmux.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/ggjprxsft.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gedblujmd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/glwrzhezy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gljrzylol.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gemzflrgx.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/ggzgithit.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/ghnopknsz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gaiyukztj.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gdyobpbwl.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gvafzohsw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/geduzlpqt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gezorhcps.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/goxfvqcyt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gmdsenqap.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/giyhqtoad.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gzkcfemks.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gguxzegnj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gkjnlhtnz.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/ghomakxjb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gwwsztkjs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gqwlfedfw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gchylorcf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gkkgyuufe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gcnofimoi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gqenwdqor.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gbzpjcern.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gyxjhnrqv.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gwgtyumxm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gtpnhfrao.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gkpqasqaq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gjhbryeoi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gyqqowirr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gmemfioix.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gvthferng.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gfihgyygd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gwxjgshlw.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gnnltypwj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gzrdsvhwv.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gsgpfdjug.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gmxcvvcnf.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/guzradjzw.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gkfhdtjxi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gdgniunqk.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gjszguqdt.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gfvxhzwgz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gadmknerl.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gxipdmmmz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glkguewbs.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcxiojnrf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gytvlgjfh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gaiqkzamw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gpivdjipr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gafbrktuo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gwbojsxdn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gqkbspkoc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/ggkhgxagq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gtefjljur.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gdfupsznc.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gxnhuawsl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gcxsukkxa.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gffcsnzal.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/ghbqmonaf.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/guscfrbft.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gdfcummmp.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/grhnskgqb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/ghbeocsnu.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gcqiqlriv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gnogckgwb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gjeqnobpk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/grglcirnn.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gowryduqt.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gyoquzcdw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gudhvjmef.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gooqglogk.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gnnqhssye.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gqhbcfwhh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/ggxdrfitq.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gvjupicgw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gwhleuzsg.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gnulbimfz.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gbfrgaxke.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/ghgfjkvel.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/ghiyaqlrr.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gltezdsnj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gbdldrilg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gtegeonmr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gugdwaxjs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gmjbyuexk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/ghnebkejy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/geaykqnub.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gqlczwdml.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gyhnyopwj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gswotoaaw.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gqhsxpren.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvxzgvqyt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gohrfeaey.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gjiyypocu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gucnmyjlx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ggmxdglhh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gndxtjrdk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gbqrxicje.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gwltfmeqt.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/glexwzjcd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gggyyapaf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/glzfukutd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gjqxomhmi.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gykmsofhm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/ghbdsrwjy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/govqhcxia.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gaueihrdb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/greqerpri.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gbodqgpss.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gzpjsaoaw.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gjpymrrka.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gzognyasu.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gbcbqwppy.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gzffnmehy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gejttqkyz.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gwdxsycvf.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gkrwbkmeq.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gltwrpraq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvhsnjhkl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gialvxhhg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gqvdmevjn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gjcmoazmv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/guqdjfwhb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gnywxqiic.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gjyanqovo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gkpvlisss.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/glfenrpzc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gycobygvr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/giuobyrtf.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gdhpocqnq.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gtqczkomj.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gqyvbdiol.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gmsqkrhgf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gdmdbefqi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gbolhwnvi.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gpruviwvg.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/glcelmmap.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gqbcndgog.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/geuwmlcsn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gkaowrbli.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gbwkueddd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/ghzqxzvwb.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gvhfgbyio.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gaabvchoy.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gjzwzmmik.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gvbaxtqip.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gqgmizoik.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gggmhrrst.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gottkeghp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gewvzktcf.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gbobgpagy.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gcyxvfprh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/guklhuwnz.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/giufpjvth.sHtML


<!-- 参考信息 -->