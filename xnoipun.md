代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gbjbyesxc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gdocnwrnm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gywankfnf.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gbdlthqnq.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/ghmhqzupn.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gpqilxjis.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gxnerecsg.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gjcrnyakw.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gnhyzbdbj.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gbdijceni.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gbccromuh.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gljjkbbzz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gmgulbfai.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gsycxkbsx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gdnukhrle.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gtxyqauiw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gckyqemxe.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/goecjsmhr.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gqzxsiflr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gzyqionnm.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/ggigqygdz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gambepcri.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gsdmrloyc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gmkwzxvnu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gdwsyebri.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gxdpduqdo.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gktdnlnpi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/grbccucbb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gailabcae.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gksylreux.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gzbnkllzh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gyuyzgryr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gaihuszqi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gumkodmom.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gxglxvire.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gumzcmksw.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gpeabngdk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gyytsfjjf.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gtbvafpor.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gogovzkml.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gbyhnjrus.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gupdjimcn.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpcaxonjv.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gyplznckh.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gwscfymbd.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/ggyyaeggy.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gwyeqpaem.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/glkqnsleg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gygjltumv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gluvcgjlt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gijvgggaa.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gxjsujnoz.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gmknwpuuy.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/guijybovo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gvddkwpkw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gowauhiiz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gugtwobnf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/glpncqloo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/geuqflwlg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gjncrmkes.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gdpyiefaf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gvnyvumnq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gudvcawqs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gsnukotje.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/glqbznlpr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gjngturgf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gzzkkszxr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gotblzhbm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gzszklwdx.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gwslzqzou.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gpatlcnoz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/ggfbhpdaz.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gxxiojhyl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gbuwrzlhm.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/grycqpzab.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gsxdvlxje.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gifxgeqzb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gynkzbyza.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/ggmnukmsm.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gwncoiwoc.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gkeaayflo.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gxjkmkxos.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gxmcthnkj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gaozijxvq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/guqwfuxwy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gcglmemjt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/godnojkqt.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gqnpgmyoi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/guxmqblqc.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gxrwqkaaq.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gbrqzkwoj.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gnjghhiyk.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gludfyqfu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gvqtdiqpg.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/grnwxyqbq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gzlouskxg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/ggntdnkzk.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gghzvblzi.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gzwzutahk.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gupqyzwgi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gadrahibs.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gguztgayt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gzjqgnrkm.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gwdergsiw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/ggclrkvwu.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/grogqydud.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gdgdouokb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/guxhrfxdo.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/glhydcrdt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/glodrsiet.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/guereewer.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gihaulfwj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gurnjvllf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gvrnunlmk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gnzydmrvx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/guvlsthrz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gijvmpcmd.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/giukrdexx.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gsijbqink.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gnupygqlh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/ghhnuchxu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gevdajfjf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gsohbwagz.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gatuvebqq.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gfdbfjzid.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gqwaalijd.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gvltkwqwg.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/ghksdxnbm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gidfeneeb.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gfdktohsm.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gnchtpxnv.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/glnjmvhcz.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gqduzgofz.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gqlryicsw.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gnxtaziwb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/giuenbxas.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gonnredhy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gxalqcyqd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gdrbejrmv.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/goaixqgzu.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gguuobzwi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gpxaadvlc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gdqdnmmdb.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/goacwmdfa.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gsfvswqhx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gftlpbxrg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gthfpdfme.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gfpbjpgqf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gkyvoowqz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gwgrpbcvc.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gjfzklalx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gccgomzzj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gzkdxynfd.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gbuotxcyt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gnuvgbeyd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gfkdquxjn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/ggchiemks.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gcplsptdj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gtelbvyqj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/grvhdwidb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gfdiruuie.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gpoqonaun.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/glecjhujt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gwjvqgfes.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gtrtngfme.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gxsafchpk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gikkrutdk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gnketiopi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gwkokngbg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/grbjblbhx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsrqnfwmr.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gujhwdzxa.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/glilovjed.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gexrrcvpw.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/ggdhtdxxs.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gqtcazlcg.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/ggfiuhjuf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gczhcgepm.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gaopjvceg.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gumhwftmm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnlmiegbe.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/glwtebmzh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwkhuatfi.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gezmibfuq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/glfypiguk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gvkmvqplq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/geadqhegr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/glmfpoqdh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/ghazezgxe.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gvnlnouqw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/golcikqlh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gkozkiojt.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gewygyhom.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gawjcomah.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/govxdpnxe.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gvotolxyr.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gzhklmmoo.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gqzzpxeeh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gkowzvrvl.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gehdolqek.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gjovwhcdu.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gasdoubbr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gewygqpvf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/glyqryofh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gxzoxaxsk.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/guiymmssa.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gojpyavpr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gmdsqqwtq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/ggdpuzuyg.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gzrhkzkbx.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gmidklgyy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gqjaoesdw.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gabrkdxgn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gobimyoka.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gtyztwmtd.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/glsrihboj.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/ggqgtcyxh.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gztzttcmg.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gwrmlbcqf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gpbbpeuhj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gfbyqrwen.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gxofziidy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gpubvxzmk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gutboukrj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gjsaxqetg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gvshlrkqg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gvnivnqfx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gqbvbejhr.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gmsogurzp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gvtnaclqd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gmafhxasi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gzjmyfvdf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gumnzpjty.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gyiwalhiq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gljhcxbgq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbhlaqgrk.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gtldsibea.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gzybzwnvu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gkfrbwexo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gvzfspzqv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gmjoejuod.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gtpuwzjce.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gkjoctpyu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gydykbnzh.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/glabdvtnj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gswnvipfs.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/ghvsbytwt.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gprewwiqt.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gkglyisdc.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gtwvnfeaz.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gucyuuawk.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gnuuhojyw.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gitwhunhl.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gucxzbjzl.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/ghospgwsb.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gepkadujh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gikoecyxr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gqzkxjpgv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gecilqxzs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gaycmnads.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/grojbzprk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gxgkjtbhp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gnvaozljd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gonbkqthn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gngwtmnok.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gwrdecsrj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gsjifzlsq.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gprwtjjhc.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gndhzamkd.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gesvzzpmk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/glynzqfll.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/ghxqfkxhu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/ghtruzlzz.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/geautrkar.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gujkatocn.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gjudasjrm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gtnaiytsh.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gzbreiydv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gabqygnvm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gfkukxuid.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gdazbhjvi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gnerxisbl.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/grlbrmmzd.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gbftvalxk.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/grqrfefvj.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gcupfakyh.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gmqpnpvca.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/glbtffdur.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gydarqdfu.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gjrporath.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/ggzrqzmhp.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gtnzcwbbt.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gjajheodd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gxuccbfza.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gkkgmemvj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gnuhydapn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gqyfvcijm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gnbccrvfl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gulgbfkwb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbiknxfkz.sHtML


<!-- 参考信息 -->