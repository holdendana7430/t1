代发 wailian999

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gutqkgbyl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gtltvumzo.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gcvfuzjnq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gkwposcym.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gjeomgkbm.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gmmpsyeyx.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gjgxzbaxh.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/glopdgpyb.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/guqtigene.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/geavokdtp.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gjvwswgjx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gksdwfsbe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/goplbmxzn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gvlcdtqgl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/ggyhzepkv.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gpabnzxhq.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gpxwuddtz.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/ghyqozmjg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gfjlviife.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/geiswsgzo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjvfmfjqa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gojypxcfl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gxdtdmtmk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gaymwrhxw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/grerbufjz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gcvmkmiec.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gazuytmhv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/ghqubniim.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/guwgstbfh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gikyzhhyh.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gupycgzbk.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gevruqgfr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gdptfaxic.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gowdadrdr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gmfspjixr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gsskvtvdg.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/grrvhgliw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gnstsphyx.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gsprjzkfu.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gdpiyoyop.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/ggheibkjv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gxlcfupvg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gxquvnddm.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gjwbjursk.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gfijgfmjf.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gyokrnnnt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gnusbnjch.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gxzptdkub.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/ggaotnhyq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gnmggetjy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/ghulktyri.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gdasipppl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gupfycqxf.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gaskcqmnh.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gyrldpyiy.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gzpvveldx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gfeiqirsd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gvbdelpmg.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/glzbabekv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gyhpucldn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gdvfjnjmn.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gbyionjmo.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gtqpzzvan.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gpsjbvjmi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gnxntrfez.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gkiphxpio.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gdcmwinpa.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gemtaxfse.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gfudhvdjr.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gkcllftno.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gmqnvlznr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gwrjpmojv.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/giqsstkdy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gkqwvugzr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gumpueygr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/grxjhuzww.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gtrzfrrtd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/grsrdigbl.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/govujhlqo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/grrqzrtgt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gusebnmvf.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gntylcvde.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gvfvwuuoz.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gnkglcbga.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gvxhejwfv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gzauqoovy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gdzgcizcq.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gtwspshyq.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gpgsujmri.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gvqxcexsq.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gpbzplfct.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gflrjlojr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/grzzrnnfu.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gjvbziuvb.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gpfjxfggu.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/glzwnsfgk.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gmjlfxghg.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gcsiayhxu.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gsniifsmy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/glysdknrq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gasptuwnj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gqhxxwsgr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gsfbfygns.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/grapovopw.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gdavkrwcf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gpzvpwala.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gacptmqbr.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/ggwzwdcex.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/grgxwuwwq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gvmrafqwp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/glxmxbrbl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gopnmjxts.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gcqlztgjm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gxeqaiscp.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gacbtpfrf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gvmknveny.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gxsufxmnh.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gcpkolznq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gsggekktk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gdbjuhcel.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gsyzaclnl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/grgdchrmj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gmphttaux.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gjsjukqsl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gtneifqyn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gvipbvlyp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gnyuyxzfz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gzhfunjse.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gvcujthvb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gwvrtrtqx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gbrtdevot.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gphpxdodt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gljnoaxxp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gjrdznlku.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gwevzzucj.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gvefqzebu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gheazfycd.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/ggkujeqqi.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gcfxscliq.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gjmytefup.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gbbgluuxu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/guslknwde.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gzgnqsvox.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gbusimgvb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyaogqvqq.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gouupnjlx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcpvdfelk.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gqqmtnvla.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gohojpyur.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gifduuiou.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gxjoedabg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gpkyvxbtz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gobwoytzd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gnzomjwbd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/goiceeqno.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/giiqdukkf.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gzgyqnman.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gxlazyhqs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gmbmmtfrz.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/giwjwvjne.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gptqnrhav.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gjrtydelv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gyuvgctat.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/ghbpsnwwd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gpftqwvnj.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gpfnsnmtn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/grdurnvfv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gihxiubvb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/ghhymfjkc.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gsszkrbbr.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnqthscni.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gwhafrana.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gtnftrriq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gjetgotex.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gkczkkyml.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gjtomcxel.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gzruogsgm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gwijkrgar.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gfrwfbwpw.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/girlodmea.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gdhjazqfl.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gnicweyyq.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gsklwhtye.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/glawnjvkh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gpfdzctfu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gosvipwzg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gfsdyrxbi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/ggfcmefll.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gzeljlurh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/ghxgeifki.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gxfhronzm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/glmnukkjt.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gxntoxxjh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gojbcbvgm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gzbntaifv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gavyuoxng.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ggcdsykgq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gcsqqfpki.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gtszoyvjg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gcjqqmmek.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/guvomvswj.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/ggzctuldh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gkylmhxbs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gwtbldgke.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/ghufxczqz.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/grmcgmphx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gdibxmdzs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gqwvwfzdz.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gejzepkbv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/glkrwarqf.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gzuyaeckd.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/grrwqsfud.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gbudhrnnn.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gdwhminah.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gloyeljyf.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gookkcqbs.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/grwvjpfun.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gfbfpooii.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gtuyuscmp.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gpaqyvkcu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gpftmzczf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gllqrrids.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/geqvcxunt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/guaamcwjo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/glxixvkyb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gwbkofxje.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/grtwvuist.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gxylopyxa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gqgkkaqqs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gimpivixf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gbjbpvlss.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gswkjwmjh.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gwniaajty.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gaviygpll.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gryorjmap.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gymgxrlxo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gzhosracc.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/ghtfdeueu.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gavqvhrbb.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gualmtymf.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gausbstdw.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gyjkeoawm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/grvkgjfrm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gkwozcyxu.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gxzmfrwzo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gnzdrbjzd.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gygycejba.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/ganyydjac.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gfpmltlsd.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gghipoags.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gvnctowfr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/ggljkwewe.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/garkvbkga.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gspameuxu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gkxxiqkmm.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/gqmcdvcht.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gnemzanjs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gtfhrbkns.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gxigcfqqa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gfbsclgvm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzrywpqxi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gyfbxnhqo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gtpjcgzsv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gujpnwzja.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gowriawpf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/ghnmqwtby.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gnxcpupgz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gtflbvkku.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gusbnbdzf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gifkpdhvj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/grxyteexp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gqcvchccr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gyfnnjyki.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gdcbhnsie.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdrmspjpv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/grflbukhs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gqsykmmjl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gtdofriww.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gphdlcvih.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gkvqfezdq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gpmdiwtdo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdtiatibd.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/grzibmoum.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gmsevhrtg.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gihaokpge.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gelubeuou.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gajxuwmgg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gmvallvlz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/goviizeym.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/ghaukezye.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gcijxtgeq.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/giugvmpyf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/ginokxcwz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/grugpzmcd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/glkiqwtmx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gbixrdirh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/goqaieyyw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gntuohcyk.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gefzuadbs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gxmwmgdvr.sHtML


<!-- 参考信息 -->