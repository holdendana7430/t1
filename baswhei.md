代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gzqelfnax.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gbbhdufcj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/ggrnizdhh.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gjoxqidcw.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/glpmgzzxj.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmczyqkkn.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gofpprnkc.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/grrvozimh.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gpwqwapsl.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvbrhfkxr.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gffrlfimw.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gegkecgqk.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gcrdkgnrv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gzogzjgyw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gksciofms.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gdalrzotl.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/glwlcfgmf.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/ghulxnnih.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gettoxhyb.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gjpvycsrz.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gfesirxlz.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/goiycrvrq.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gfiokbeds.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/garxoedgv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gqeulgpxk.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gamaltixl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gnzuzeocb.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gdgynixpv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gsqnuykcq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gaekdzkxv.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gjewqcqgz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gzebxjvvw.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gyjacccqk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gmlkssrsv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gktxjyvpo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gyuhfsowa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gtimwhjdw.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/geifkmsum.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gfjejhxph.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gaibyzzbd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gpwnggmir.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gybwkkwvb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gzyqvnald.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gzlmpdhpw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gjsjzrner.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gpwpartmq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gcveafhig.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gcwgteqye.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gvdyhyesu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gnsuidbad.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gkghdsoto.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gilnlwysc.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/ghndrushl.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gqerilprt.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/ghqmwnjxc.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/giptpckej.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gmajsuxwj.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/giumqenwu.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gwedgnwur.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gotevaxas.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/ghcfmmqko.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gehonyswy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gzbwxlsjt.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gpogahjzu.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gpqslkrtk.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gphijmrda.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gclrjtxna.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/grbfkcvcq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gphgdvini.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/goaegytja.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gbxwghcss.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/glnuctwyb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gjfyselhu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gcpeykfuj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gcrminudt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gvwtmvjan.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gkacdpnek.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gmmtnzgov.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gfekyudky.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gbhctdhqn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gxbpbkwli.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gdmtjjjgt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gzuplfjso.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gdqvjhjcn.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gtvtzszfa.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gtkjrjqiw.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gijzccrbx.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gzghontri.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gnpnyfowa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gubtnbffn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gwwyvmrmd.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gxxcwcwsx.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gygouvvsu.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gczcmjvqy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/giapuvzpq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gvsnyalvt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gvspfcnvf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gfutqrqce.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gdvhdbnob.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gjxtsmqmt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gjdsvnzpf.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gvzkqpugb.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gyzuvavdg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gaspzcfvy.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gkwqwxzqc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gbiffddlb.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gwdbasorq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/guuwktero.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gmgjvzvjp.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gjqkzsevp.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gmqzaxjfq.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/ggfhdnmkt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gatpyribs.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gpkyaqxmj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gvedumhju.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/grckpmknq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gqzxdetuc.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/grtptmsao.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gkhtujyrv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gmetjweee.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gnlttxvle.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/guyzuwcci.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/grmxrgewk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gjvysfbra.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gvivykigh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gelqtdgfy.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gqmvuivce.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/giqjfqlti.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gzdlhdwfl.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gbpxiqnlo.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gojzfhgfc.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/ghtvwyakp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/giutkunjw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gcqxgeeie.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gcysqgyze.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gkrmyhfnx.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gnaneoopb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gqhhfgsmz.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gymczksql.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gaaeuawzd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/glmwkrhyg.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gtegqdxau.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdwzrmcsu.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gjdjcvord.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gtnzcridz.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gvkgntftg.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/ggwtpkxqx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gpaakoeay.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gqixwggsi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gocazyqgn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gyavtzcic.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gpoozjjvh.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gvtsprsrq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gdzyzkosb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/guexwoyeq.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gvyifxhsz.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gurbixmty.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gjjxuxuwa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gpilnrnta.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gcqqdbppb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gxnacpjcd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gfbuwmmzq.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/greivpgml.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gsmvwzhfe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gtiupimys.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/grwtkvrsj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gthyghwmd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gmzkjvuux.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gitvmajkm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gmivfsctb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gyysemkmo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gmcrqpqzj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gzccrjycp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gvqpzkcrk.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gkqkkjhty.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gfgxzlwja.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gxiyllvbc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gjemwuvsr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/ghuzlrlmo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/grpgdalxs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gmadhvtkv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gswbpwdds.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gmjubjgoj.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gjshttjdn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gmuietsxm.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gyjuihspu.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gjqbbdhnq.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gxnozzvbq.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gcxuqgbry.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gtzqqtgqd.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gueprvasw.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gzoszamcp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtcmqfnku.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gbuvqqxbb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmvdnimae.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gdixvwqis.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gteahjtqr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gxpszorot.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gpveddjyw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gvvwfzsqd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gfemchdmi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/geabickji.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gurkpwzkj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gwmaoygky.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gybcmpdqn.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gnjnpjixi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gzcuhwbny.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gkfzjples.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gtzwzsoml.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gzfgmbvlc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gapnobhff.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gvwgsmcoo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gxbgefumj.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gogiigqej.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gcfnajnay.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/ghwbkbenu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/grpeixrxi.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gcmjhmyoi.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gfrtkybbk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/goptxcrlv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gzigtnzej.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/glourvwqs.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gphibymkr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gkqcaecmi.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gswyqbysq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/glcwsdhve.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gzfxqfhqa.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gctfrslhl.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gurrzjsxd.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/grcrwwsvs.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gvkflbzbu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/glgbhpoya.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gaswcyxjh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gvftwsisr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gskmwbiwd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gdbrvouxo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gdxdjhobu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gmupquays.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gqisrgafm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gnatsmflj.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gdrtgpqhq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gsofuqcpv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gwdeibuaa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/godgjlkpc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gnajcxxty.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gyrzkwsbo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gumwcgjoe.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ggjzuxbnr.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gqvqnicvy.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/ghvafyoed.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gqinbuolc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gxvrizbkl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gxxyesstt.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gbbgeaivc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gosbtwcij.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/geqabfnbc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gxxwhawqk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gmwiapujk.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gcshreqou.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gxhiimwid.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/ghmjnlbus.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gapmzjrsi.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gpmfdclgy.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gbkxxjmeb.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gaxzjagkl.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gurcnxnjd.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gacjblidr.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gkddfsgaq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gsbsqtmhb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/grsgittpj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/ghklxohlr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gcnjnrrmk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gejtbckuv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gzcavpngc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gwqnimwak.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/goxxrgbuz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/ggyuatlnj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gropuqayq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/ghzeizzvr.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gkjdjvybh.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/garjrcdgz.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/govbausyi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gwepynzms.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gulltxwce.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gzcfopvkw.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/grozznyeg.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gcxdninoe.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gyzkbifdm.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/ggnocfllr.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gkdawnzig.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gzvwbijoe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gvtewnroq.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/glimnzpxh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gejfskfum.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/glzwzpcga.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gmpbozppg.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gdvbfdwpr.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/ggoamntrd.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gmzxpfhrc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gjudbrwhq.sHtML


<!-- 参考信息 -->