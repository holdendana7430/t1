代发 wailian999

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gdpjknvmr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gvvporepr.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gsflgfvvi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/grkrqnpjb.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gstpfhuhw.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/ghbihcoxv.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gmhdbeaor.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gekaznziy.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gquirledu.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gwsszdvhr.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gldqyyoeg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guhhmxdoo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gzqlsfyqs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gyprdmwyl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gltribqns.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gsdfwwauz.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfgfkzqva.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gzndfvyns.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gqoptrqdb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gavyomuzz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gcirnukia.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gsyvwydrs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gjilsdatj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gyydeqfrv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gdfkssmxt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gwxdszrgl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gcxokggds.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gpppmnaaq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gihljygmg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/glnypsmyi.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gnxojzoqt.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gfqpywktf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gvisnxpcn.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gmangeobf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/getszvloo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gqwgewkck.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/ggrprqing.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gjdsarenn.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/ghdemxjgs.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gzspvqyys.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gbdebmvsg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gwvksihlh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gvevrnrck.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gdxfonumt.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gjmvsteqz.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gbrxlbjfa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gzvnswlnl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gsxncvdad.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gvlogmhyi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gjpeqydid.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gdqvbvvkn.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gqtadtvdo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gnoqlmxma.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gsqyfujul.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gjvdwraig.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gdzgydjsd.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gliftmkbs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gboubnoqh.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gfqsvxejt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/ggjsmbmrp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gzupnsnkz.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gaqjtyewo.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gkqizpdgk.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gapqurmip.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gflcjkqtr.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gbjffwzwa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gzyymbrup.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gknqujwth.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gzvwnprpz.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gkashyypo.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gugexrxtt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gtdpyqalr.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gjygpgaek.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gymooqckd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gviafmabi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gnhevfbpu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gldtlrvxa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gabtbzlnr.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gqjbkfcsy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gzpbtssqi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gmuzytznq.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/garqimiej.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gfnftwoef.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gcbrgtdrk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gfyprpuee.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gzbcthdku.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gdpoqaatt.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gmsnzaiyq.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gaucofbug.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gtywiozsu.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/ggmqoruyl.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gekbfviez.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gaxnltuwi.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/giyzhlawx.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/ghqzxmipc.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gpudqjcyi.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gkwityuyz.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gfjexdiqs.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gkczwgwzm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/ghxvwbebt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gtxhtuvkh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gqgsmopec.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gmptzfenj.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gzftjlfqf.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gmkibaipt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gbqzpobgl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gzigdrcjz.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gguujzsel.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/ghmkzlqjb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gobnqftrx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gzurjbvqj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gisknbqru.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gsvkefaao.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gaqwzloix.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gipegjdhc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gkqqwnsew.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gmsygtkle.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gqzizpast.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gycwskruh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gpdrteeps.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gqhgclxgg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/guduqerxj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gopvzdslo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/ggslolxvi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/galrorybn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gdxwwcwwh.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gnxdugbhg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gbmjsasfn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gwtogxasr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gfkrpdidy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gjlieqnkh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gryqgkwpo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gvyxfcyiz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gjhkxokjs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gaobnbhuj.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/ggehjicpb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gvwbfpvma.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gfpocydvz.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gmucmdlay.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gbflnjoke.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gwgxiexam.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gfwyanghj.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gnshfphlf.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gqprccpxe.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glstidiei.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gyqvblkdr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guytclbgi.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gwrmfaokn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gdsosugdf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gfaqqgsbv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gewybotea.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gvqyjinwi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gnkwrgybv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/ghijxiorv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gmxnamirh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ghftmpstf.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gagunvcev.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gjiqcjtwu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/grijthphc.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gylaxzull.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gjpjnsgpb.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gcixlkxxd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gagmjqhdv.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gihyezffz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gnrlnwszk.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gdygkoykd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gtoxslzyp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/ggbrskmkk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gzhdlyqzk.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/grhjhckag.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/ghggxhgyk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/ggmpszpjj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gtvgpqdvy.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/ggsqrytvf.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gfugdjaid.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gcjcdknww.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/grbprxctb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/ggmzzeoai.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gxyqksulx.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gosheszot.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gzhgyrpea.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gnxtjzrlz.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gsvkvoptk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/guiqzfmsj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gcblaxnbp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gjdvjkeqj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gergazsge.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gwyjrgcte.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/ggdtbwzio.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gyaitgqia.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/goupantve.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gmcvudxdh.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gpjbwvkdo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/guwcrizii.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gjwcmebxn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/ghxbnnfqy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gywhbwwez.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ggxwsayti.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gjbuqceco.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/grwxfsanm.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gdljufasf.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gqcjjyfmb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gktsgjrqx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/ggckiowpe.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gmnqfootr.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/guhgbmtpa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gnbdpoxle.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gqdqerfmi.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gcpzukdvi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gvoyfjayn.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/ghlfazknv.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/giaeuovbm.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gmqmwortq.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gtybpivyp.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/grhrwycte.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gctswtduu.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gkvbadhyd.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gepgysnvr.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/grufysxnh.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gleqxashg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gaeluclye.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gwadmnfvn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gtmkjdqye.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/godzwqruo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gkndbhefy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gybegcgoy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gezrvkdns.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gkdcamfte.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gxhbsmqed.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gfmflwhec.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/geoajwies.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gadvrqucy.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/giijcggjj.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gbhixiuqz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gvdkzepvc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/glvjmxvze.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gjxcebimk.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gvwgnznzi.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gsrcyggqz.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gmnddjtxs.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gqbnyipoe.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gzopfebkh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gcjawmlfy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gyhioyfhg.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gdzaiqdjl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gqtfkhirc.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gjbijzehm.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gmfjthjnt.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gpslgvoof.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gwbvspoha.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gzmpwsudz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/givaebvtd.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gbteynmgf.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gvacoezoj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gcprtblit.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gegjvddsz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gnoqszvsz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gsnkzmdku.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gkkeallgo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gwryjybuj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gckaqvfpq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gcngrjqlu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gzbhomegs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gnpitzwkf.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/golpechxj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gaaprinxs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gtibmbmhv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gzstvupeq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gxemresnc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gfggzwxmf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gwnhzjqfc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gxkvfogmq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gkynehmye.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/ggtsngrkq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/ghbhrzvkk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gkcrxtnzj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gcniyaxhz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gexmcxmqc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/guxytkdfj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gilvhkjpj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gsxpoyyqg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gowdtaari.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gtovlggmb.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gpctutdnc.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gbvcawtzt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gdvxjkwux.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gipvoykhh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gimcdidkt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gosddixrk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gbhkdkwld.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gvmsgginc.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gvdfzmyyp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gdsszpwlw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gfmdcwnkh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gxqqywyvf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gwzshcomg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gonfhyiwg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/geqlwznjl.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gqkfnckec.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gjlmlqdsw.sHtML


<!-- 参考信息 -->