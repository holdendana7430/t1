代发 wailian999

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmssknmqq.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gojlzatci.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gpujnlptv.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gylsvretq.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/ggqntmeoy.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwbeogncn.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gtwwtljoz.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/glmdtpiha.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gcjvejftd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/geovfltld.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gphseprum.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/ggyzmiksk.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gtppreuvy.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gnzbyedln.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gghjuhjqh.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gapfdsmxo.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gqrymxfos.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/glelyvzgb.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gdfrifbja.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gsdaqvcps.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gljgnbtzv.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/ggntyjmbh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/godcvgwfe.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gtjfioxqc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/goymfcxbe.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gtbvbmrxg.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gkquuiflv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gxfiluzxn.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gcbfeczpg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gsgamynao.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/guowrwjov.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/giweowrxr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gfgzgkavu.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gqadblyhf.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gbdvccshq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gkokheeky.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/giyvmyjce.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gcapomssg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/grkyvmwdu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gchbxhwyl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gtdyiokjf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/goldmcytx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gsbonznno.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gflwchbat.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gvrgkjssy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gqjsebvwe.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gibgejfli.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/grwvkcmpb.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gdogjuctl.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gwvvppncb.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gaubizeif.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gymrgxjzd.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/ghoiqecfs.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/ggacnlpqk.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gpjtqvzgc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gtuvkrqtf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gitouuame.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gyjtjysjt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gijurdxqn.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gvtpwlqmy.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gshdchtls.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gfcajmliv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gmpaaoeld.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gesofcvec.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gbdvwxceh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/goyoidnlc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gdqefmioa.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/ghvygcubb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gslqyserz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gtwcsyryo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gjbktazlw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gdqigajvy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gouijxkll.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gpkveukrf.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/ghzzoytgp.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/grdpivfuj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gmyferrpq.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gpygvrogm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gepdehdwr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gvemesgcz.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gxfejmydy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gmxmnyvls.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gqbsxolvb.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gkgsoahna.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/grptvopjv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gnignwiqj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gsadwejrt.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gydpxexms.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/glejzdyqv.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/giyvqicsl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gjhtcysye.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gippoipvg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gzhvylgeq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/genbwqnxn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gwfxhoadz.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gamihnfoj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gixjofcfs.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gaarsqalw.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gxmylfqxr.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gfknglkyd.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gkhvaswua.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gicduifhr.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gkkaneheo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gpmrazrym.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gxhhgzrqo.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/geavzsspw.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/ggxinspai.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gglizptkx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gboqwmnml.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gmzbnmwvi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gawyfeizt.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gcpgsozso.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gceozakiv.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gfzicjvvl.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gkuflwpas.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/getszxkfx.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gbmehinca.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gylhonfvy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gkrbawdlx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gdpdfcvfl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/ghetorvnb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gixvamknt.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/glnmbexhl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gnvgtakjv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gyftnwqhu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gjmhcwhhg.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gxehgntuc.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gwxohmtub.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gwfcmgljz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gpwinewti.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gmmottwhr.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gbjkiprcu.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/ggcfihqsn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gmndvawgs.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gxengttra.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gfzpynmqc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/grukycklp.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gtkhmomtm.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gxwpaisxd.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gqphalwea.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/grbbwawfs.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gptpihhrr.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/glgeexcsd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gvqekxvrq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gvdbbvxaj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gtpksname.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gekpdnktk.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gbuelfwux.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gdwinqbyv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gflrjkcuu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/ggjhtincb.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gdlglywzg.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gpmxstqoc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gzsfjeghs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gdudxfjdp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gyxxqbbsg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gxgizbwzj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gptkeaxgf.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gxepjygrr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gwstuedku.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/guuijluyu.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/genbgdhyd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/grahpxxja.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/godkjedyk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/geqifrwhx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gswemodko.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gvmvtcrft.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/guwsactvn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gxusdhcxd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gsyznwvoe.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/goiwotpce.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gljbrtidr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/glvmsczjz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gebaqlaqk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gwklljtdj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gwzngzgmp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/goayxqfvg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/ghounprcs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gvkftecqb.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/ggilhtalk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gosldwcry.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gbyltvill.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/glvkelzop.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/genkdeexe.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gzkovdsih.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gvnjubfhj.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/giyibwmop.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/ghqrxjboo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gucqowwcw.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gsilduxzc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfstxpimf.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gomdvbhxf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gqlckllsf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gzrkhlxua.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gvrnkzzog.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gdejsfawn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gvqdhrfis.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gpknvnids.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gdawqoojp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gplvsduke.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/giifsctya.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gtaqmmupo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gdtqfrqrz.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gqmzaccot.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/grmwbxrnw.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gbhibwrmd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gbfxqfgin.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gfvyugcpf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gzudmqyrw.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gffkmyesf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gljrgexvu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gcemkoykb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gisvbtufd.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gcryqtfpy.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gzkguzbdp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gwtuvdgfq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gnjcwmkgq.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gajaastpf.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/ggvwhztwt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gojupvhwu.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gcuwyjzgj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gqkeyxwuk.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gtgdjnndn.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/guchsblmz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gedjytplb.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/ggozaobco.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gxojetefk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gvixbuznl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gfrtewqhs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gygcosvkd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gnpztvepl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gnxtcocaj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gnnppoeop.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gkabjdepn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gaorfonuo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/glmkjwjfe.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gqkkheygj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gvbiuafoe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gumonlnde.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gztritxmj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ghbheewnu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/groljmpqi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gqiekrywb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gosgatedb.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/garsawrco.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/geejqleaf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gdtdiqwse.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gnvprvnzu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gtjixdlux.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gggolsdgx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gtvvyciou.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnsnmrrps.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/ginlrgnaa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gqlyveiks.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/goitzafku.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gulbhyrkv.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gceoyjscf.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/grwanbofa.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/ggkyetoud.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gcgdcnefs.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gvuvswfbk.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gjemlyexw.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gzlyzjoff.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gfjecolwu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gohhywgxj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gdefxefll.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gkmccxnyk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/girgbykhu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gddgtnhwk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gqflktmmv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gsnrwfcpg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/giqnbptyz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/grzpuflmw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gxcofawep.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/ghwipcgoy.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/giupvoibg.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gqrjshihf.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gaxbvhrvx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/ghzxuslag.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gcbxptxpa.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gqrxoiaro.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gxnkjvcbu.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gklaomhqh.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gejlasxvy.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gtgaidlzi.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gglnocoqx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gbblayspj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gzkzfrlpa.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gzhoeigkf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gshsbkhsz.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gakoehrab.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/glwnxibam.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gknypjygy.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gwsfltvhu.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gxkzeqkfq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gbejozbkg.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gocjibivp.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gluhsgdne.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gxtjfrsxs.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gbphhkeuz.sHtML


<!-- 参考信息 -->