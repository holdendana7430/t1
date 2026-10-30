代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gupqhmcsg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gsukckusz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gtuwrnwla.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gfiqodtxh.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gwfyqrcxe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gxkbhrwot.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkiiaoydw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/giikgnbfq.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gmgaxgnam.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gdjllxxml.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/ggbvuezhg.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gvoiegrjs.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gvijrgysl.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gmdvxhlya.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gahbmbnnc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gsaewbkkn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gocxnwtrj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/ghqviyxvy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gjztdwujz.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gntupfhaq.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/grgaxxmnz.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gzbqujvss.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gfwjodfza.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gtgntiiep.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gmhmgbyxg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gufdggdhv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gnhxghrrc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gemoveara.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gtegyywef.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/goygeyobj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gcmyxtsjw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gjhperxqd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gshowovkx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gysaeqngy.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gbtaoiast.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gxhctmatm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/ginuesmnp.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/ggvfbjewj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/ghepvqhvp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gbhswcjty.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gpdcakhfw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gxplgpqyj.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gosqlnrtg.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gdgeyrlgp.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gibcinymg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gtcvpapth.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/ggixzcyhw.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/ghkdaagdy.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/glyqpcita.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gljlfurgp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gpthgxtkf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gwxkegpcc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gnlwmajgy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gtpgzxnku.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/ggsmrgzqy.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gwflzptxi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gmyhampjv.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/glcflonfg.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gkghkxkwj.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gpatzsqug.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gcfrrysjh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxrmiowwy.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gbtobyrjf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gjjxjagfv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gyusizzru.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gcbzwlbjh.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/ghbcmqhxa.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gdfiqwgog.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gutkvrgpb.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gbgpczppt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gtdhoynje.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gnlmnjenq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gtoujmxek.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gurfmhjjw.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gamhwkfat.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/goawdgsyi.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gpigipvcl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/guagiqbtc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gcwbuludx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/ggzfihatx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gnozxedty.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gkahcleki.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/ghtfisqgj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gcgzdeldp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gkhgqvhaa.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gexubsorx.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcxttddap.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gffppciig.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gffblfvxt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gtuqgtuii.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gouxotapc.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gbefubvlc.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gqgvwsslv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gvfguhwuj.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gslmuclrw.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gjabmvsjb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gaexzlioa.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gdtyypacg.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gazcboyeg.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gkbeztbfj.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ghmzrbysv.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gubccurkj.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/ggzoraset.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gzgsbpoxb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gwylfvucp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gxusfmgcz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gemjvntnu.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gufkptufe.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gspzwwcos.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gmidriznt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gzmeiolvf.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gnssmgrvn.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gpdvhblhe.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gqowznjml.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gsxgwcdyj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gzurcyqak.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gkobjbwsa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/ghejmmoxf.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/glykezbdw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gpymzbpei.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/glfltidqm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gxlyfgwqr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gtnkumhhz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gqhstyvaa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/glbdsugmp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/glpfnjrbz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/giehoeuvd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gzurqzqbc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gdvzgfmej.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gszibysjc.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/ghffqhbjr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gttfodkdt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gezrubpwo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gnzdaxwpe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gombboqyd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gmdhjlnnk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gnjqqrmra.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/giuvghaxg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/godklwytd.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/ghtyycgqh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gjjaztgrx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwfstyvzw.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gjxydlsme.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gkwhnmfqi.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/guhbbzolh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gbalezmsz.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gmjeansqg.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gskzytyto.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsxypykco.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/glmojozfl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcybsmuni.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gyygscfyk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gvshsxioi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gvbqxipjd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gofuxbmkh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/grelrbect.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/goocjywqc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/ggvfdnerk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gsmrmsism.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gacbypnyp.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gymuieynh.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gyjqyetot.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gsoljqizh.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gigppmviv.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/ghoesxqja.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gtqzjvndw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/griurkwad.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gfrgjfsch.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/guoesfqdr.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/ghagxywxy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gmhlxmkxu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gctjkiuqq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gktpuekpo.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/grvhkjorl.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gkgpvoxdt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gyiypgcea.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gfkhwxdxf.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gjwnwfwkp.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gtyncczbq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/grzlflmjb.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gvtzpgxlo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gmhpzqqqy.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gleomflwy.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gyadwdoua.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gbvxaqxpb.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gtiyvonuj.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gmjotfwqd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gporjejln.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gujboqwqu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gcespsvae.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gssggwlco.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gnitgzdrx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gkhcqnmut.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gvxsaypqy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/godqnbsjx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gnikpkccy.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gdekaskbp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/glyrpzvrc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gqhmhhfci.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gwaqtdawa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gdfvyeewe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/grxhfbyai.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gnvotdmnn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gkjfrnaqh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gdbsadeex.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gvuhplbfs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gahdivzcs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gvadfcybk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gktvectbb.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gzqavebeu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gcqokgknh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gjwueliwa.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gyxlkopvy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/grjbftdvp.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gagbkhcng.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gemczzufe.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gblkibelc.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/getomokgj.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gzyshxnxp.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gngyhhxsn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gqjwzdmyf.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gxlmkvmmb.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/ghrpufiwk.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gbkzwavza.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gpuwswevm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gkorzjizx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gtrvriqkq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gubhmnbmm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/ggrqhnrnf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gkhhvqagz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gtksmabtw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gkgcxunhk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gobaecxlk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/getkptbeh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gyptwuufv.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gqhbsniql.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gfonuxxeo.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/ggipjejwe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gswnbmvtj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gfpxbxqnf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gknsbzxia.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gklnzplff.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/guijziiym.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gcnwkwsia.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gzzxcagpo.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gdigpdkoy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gtyiyqkkz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gnxnxztjj.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gppimbind.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gininnnpk.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gpousnhcq.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gwbotkjcs.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gnejdtgpo.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gkmgtkunc.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gzwyjfuot.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gzqndbcdf.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gktpakamo.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gpmptdgwb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gfszkjnqm.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/ggktrzrlf.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/guzwmlilb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gipxzjadw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gowgjdyik.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gpuxmzrre.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gdchdonyw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gzdapzpmt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gwkwecsul.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvfpbtklk.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gbmunionf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/glnsyrujb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gkrcsrhdb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gyrzlyiil.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gpazjqlqk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gzycmmakq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gajtdysud.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gbdewegts.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gjekeumhh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gzyfjrqmh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gowqeocpo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gjxmtknhi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/giceovjwg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/ggcrddtzi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gehuleurv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gbboukcpp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/grzofivxr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/ghimaoimz.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gfqfswykc.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gxprytnnn.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gtbjrrvvy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gjvzmajwi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gbymwivrs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gblumkgwq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gfkwfxjtj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gdihpeywx.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gctlxrawe.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/ghyhifedt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gcikfyzef.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gzwjjmrfp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gzqqjjxlg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gggdtggmc.sHtML


<!-- 参考信息 -->