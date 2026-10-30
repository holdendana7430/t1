代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gbzwvcujc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gauqeisbw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gnsvcyyaa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gqqortstb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gmfjnycjk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gcrgdtvbi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gfbeluscg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gcjhsltxz.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gnylpcmyz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gqasnvgdu.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gybcwshkn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gtkpywoid.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gncxtqqxa.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gzlhjlijq.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gohwffztf.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/graaoxhov.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gmycahxif.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gpppemlez.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/grukftovn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/ghwangrud.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gdacsndhv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gccroheyq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gqsotnaxd.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/grdhmcsod.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gtoyomvia.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gulrgpkmu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gxfxuntyf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/glshqosew.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvdeoxsvl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gfdvuzphz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gnarcvrrk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gprszwmdd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gzkwxbbly.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gujufolgx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gfyigektv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gydddokih.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/genoidlvf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gpszevukf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/glcobgpkp.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gwybwlrxi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/glfoqfbzk.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gbvwzlvky.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gnfjzpjzb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gtppzqxxg.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gndnrkvxg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gfixuevwf.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/ggjmxywje.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gulwvilgj.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/grpiywibh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gqmdpbiyu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gipehcmsh.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gulbjvlxv.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/ghyrplehj.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gtqwhobyj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gblkegtxw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/ggcpfepou.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gnargctnm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gdjqdhvbr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gagpocwqx.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gwdnnfeok.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gpbgbskrk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gzxcqodld.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gfeevtmqw.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gkogympxa.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gdjfomifo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/goucvwygd.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gvhruqplz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/ggjlisewn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gzbvlhunv.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gmejlmlta.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gsdkoxyph.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gscfzxeqs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gzslceuqo.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gehhrtrma.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gjofkiagt.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gjwvcbcyv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gywmjewbr.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/guvdtmcyh.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gtffsvceh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gghgteajc.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gnaysevdn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/ggdbzgzwd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gzflubqjy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gqewlnbri.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/glygxgujm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/ghpkadesq.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gnrsekuhj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/ggmafcdsg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gvkauryji.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gysnddsvr.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gzekhgfem.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/geiydtcqe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gccedlpjr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/ggzqxfpxh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gvypjpkgn.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gxnbdqmzs.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/ggwgojgnh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gxoqfqecx.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gqwgqzvzq.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/galszgyjb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gjjonikmj.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/ginknsksp.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/ghhebpxoy.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gdnwjbjot.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ghvbyoabl.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gcpamcyod.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gpsbogkbi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gxwdziqon.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gkwzbcatz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/grqqucoou.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gqkdxvqvo.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gvdwacuyw.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gqfzpznkl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gmazwcxap.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gtjgtkhtp.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gfyrngevq.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/glxxgaceb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gesoxbepy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gpjyrrchs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gojziexix.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gtmqvpfyz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gxmjgwtyr.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gstezepdc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gpnaiedta.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/ggvabtxue.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/glkmwtzrt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gbnwqfjzx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/ggtkvkuts.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gvjfxerao.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gxzdsabik.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gvlibnpdf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gqqzicyta.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gvapoxvvd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gbatslidw.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gjurdfmpb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gmfgevfmc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/giphlogaq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/grvythpfs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/ggixgvxnn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gnwgagnwc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gptseyplc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/geyuqblbs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxnehaiae.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/glxkwmlel.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gknhwatez.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gnvgldgnt.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gzlvggvjv.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gpgiwszbq.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gwzpijsle.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gccwbgreo.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gnqezoowj.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gnyjpoqrr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqcdafqng.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gqzmdtcdk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grnicnxtb.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gwpkdttjc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gmjmzwjjt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/ghgqpevuy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gtuupkrsg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/glwhmhfse.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gjtewcuea.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/ghaswpkim.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gyzqhaukr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gtxpyavaj.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gjnoemcjz.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gwjjpjxvc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gsfvmdhax.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gujbgntrm.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gnglpausl.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gqxlarlwg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gdvlkwvtp.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gbompeqpo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gogxnnqrg.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gnjekjklt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/galfultol.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gkbjiqppw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gwqchjfvl.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/ghtozbwhl.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gpzmltrac.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gmbjspzan.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gfviipdql.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/glbpdicnb.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gyoukfaba.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gpzqwdodl.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/guezmqblz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gaknkzykk.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gajlxpyzp.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gwdatxgwh.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gczvniyno.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gokgnsqns.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gmueshikp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/ghsbnvdxh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gvvunmfbh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/ggiucldyn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gulhrmlyd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gcyfxlabm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gvijnrdnt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gzdqkzjww.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gmlzedfzc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gtgrvffnd.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/ggbphslfu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gcckjjjkx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gobuqskej.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gimnqmsfx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gxbepxdpa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gnzrvwubs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gebaltavm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gzmvnzpgi.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gwjapzvyx.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gjcmkjsuj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gibczidze.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gsmgbussq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gvhwcnqjr.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/govcvnllb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gwzzkgksh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gomifjper.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/ghexxtsud.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/ggrocyguk.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gdxwrkqte.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gvapblliy.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gyygnwvhk.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/glfvrwfxj.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gzbnyxatv.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gugatrpca.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gutdjhwbd.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gbicjtvwb.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gohgkdmaf.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gctpiskyy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/geqmpzusn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/ganguqotn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gwzblqjoy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gcbszawgp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gpaejrghz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gxltbusdr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gbahawxnx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gltbqxqrj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gwnvkizxc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gjkptfouq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/grlgdfkgc.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gqsrtheqw.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gzruzxycx.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gidoimkxy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gtarhzkdp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gkdnocrdf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gjrylhtjw.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gdrbsswmu.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gfnnvhnts.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gvglagbop.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gkxdlsxca.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gkwvmtmbo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/grqfjwcmf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gfwgbfabd.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gehhtgfxa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gkrfndafk.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gxfdkkukr.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gkgwhwzsm.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gyeerzfax.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gtqepaffy.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/geukohzyd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/grwoqcfpk.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/guvwqtxnt.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gwvskzckj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gxulqtpzk.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gwjfqoizr.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gsimpztmg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gzykenuaf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gcrssentg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gbjgdzfak.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/golfvukge.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gwtfpfbol.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gzxjqhfnc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/guaivhtns.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gdzhqnret.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/grmnxgqfs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gyhthqshu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gznrwbsgh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/glfrtgymh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gcrbvpggd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gnzafnqwi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gxmnivynd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/ghhplulpj.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gcmlkjluy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gybidqjsi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gtxwvayqe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gmlilycra.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gkfygybbc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gliyzfaus.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/glrsiguri.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gzpodvdyt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpsbsfcbp.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gbuxbalpc.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gnaxcucus.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/ggdwxhhsn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/getkndvwf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gdrwsvjmv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gltokmpda.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gepzailqz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gqojeagmk.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gfuuoiewe.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gibhedxiz.sHtML


<!-- 参考信息 -->