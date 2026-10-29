代发 wailian999

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/geudzxusj.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/geldhteuw.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gjbfsygxw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gbaqmvlpt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gjalcllyl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gbsqdevpp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/govqyazti.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gtcjomzpf.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gmlbeslmn.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gaiwoqyqj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gxtznivnf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gfmimpcqw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gsfbzsubf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gyeeqtbmg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gtrznxvkt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/guaeyjltz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/glsupmnbt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gmtjfgxlt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gnwmihjiz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gyghoccjm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gynuuwjww.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gaplhsnvn.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gfqwjwypf.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/guqlqnkez.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gjwctrddu.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/ghapkblaf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/geffomeqj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gualrlnru.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gsmnhrzbw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gdkzcqjhg.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghxxozcfi.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gktykwseu.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gwzooqppj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gdqitbxse.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gbspeiefm.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gayglrsjx.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/guumkzatq.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gtwlrefth.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gdevfovyw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gjicgvuhv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gwgibdglk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gppgyoprt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gzgdsxdjf.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gndcllwqr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gqocmrumr.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gnrfzmgam.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gosjvuolv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gkysdcref.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gtjtglpxy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gbctpaljl.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/grvvmfmud.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gbufkqqrb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfytefuos.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/grxdradlo.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gjcoyejfh.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gqbzcsawg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gkmsdmexv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/grjahibah.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gzigbpota.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gevfsvano.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gfqnyzbdt.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gbnbpgmjv.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gzzkznkrx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gezhgzkur.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gsbmbvcsx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/groramfwe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gyagtohpq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/guwsbfqst.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gfpdwvdbt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gxpzbchzk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gabsjqlpm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/ghwqeqdes.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gyeemtjmr.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gfhiibcrs.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvuojsnkl.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gtwjbzbvl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gibndaqkx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/geztoztdt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gmjclduyo.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gyudhkopc.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gmswbqyah.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gebkbezsl.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gcadwlvqf.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/ggirfcduw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gjnklfibx.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gzgneyekf.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gxaqhbwcc.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gkdqshdpm.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gygdrfjwk.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gjafqgzle.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gxztqthss.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gsemcgdot.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gbbmvojzn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/gufflatnd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gfaoonllk.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gcebwmacf.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/ggnfhsgqf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/ggqlabdzx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/ggrjhwcmr.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gxsfchulc.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gtivvqssc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gzkplbjfh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gesmgkgus.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/guhkkight.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gjrmshgoc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gpzszycgn.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gngbhdrgx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/glsldjtka.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gfuqeqjkd.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gyxeduyje.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gqjijkdde.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gdjnbqumw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gnncdxnns.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/grthdgrjy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gkoaqovzk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gvgtbjvog.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gccbcdgii.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gspwelcrv.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gddgewoki.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/grcvtcenm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gndrlrjin.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gbnmrcnjo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/giwgoafzm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/ghozvbrvb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gpxfclzdf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gqlqyibal.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gmjcqsnxd.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gqfewjple.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gdmtwbpvp.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gneydvtrn.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gbxnxebig.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/ghgobinoc.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gkxfqbisg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gpvrwclst.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gukxelrtl.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/groeljrtz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpccwwusa.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gmpbhsoon.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvoliwhin.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gsvuotzvz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gxddahixi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gxpyaexfs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gmwqzysxp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gsmtfppbd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gsqtzadig.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/getcgjfht.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/goktgpsqy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gtfbpvrnn.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gzgdhywjj.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/glncszvkh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/guwistnzl.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gdljlzzqi.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gvhopvxwc.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gyghrzwab.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gcvnwxrun.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gdsvpgybi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/guzcddrha.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gmxxrjavq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gzgsltcch.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gxherlayx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gwwzwyduc.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gxdsjaouw.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gjxpgchko.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gdmmaukjv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gwgedslqb.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gzjfiawwg.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gdzfqxtpc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gkqompcpd.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/giglfomow.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gxwkjvxgi.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gkmbdlgvw.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/grycupqzk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/gumycreka.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/ghclmqrwb.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gtuubjeoa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gwsedwzgz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/giectiiiu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gwbcexmbp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gdygpnsdo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/golnlchbz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gjotwfqal.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gyaznduap.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gosbkcymp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gsgisifox.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gesjxldxf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gduxguutu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gattvcegx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gghyolkqc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gogazgleu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gtbwjylxk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gteqgpjhl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gyiakitjo.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbketixfk.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/ghaqlrkkx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gtjoqhifq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gvguraryl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gtwrkniwk.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/getsfvivz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gvqyjtwtb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gknvljdnf.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gnhqdhkpl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gvpieivzk.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/ggvtzmtxd.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/guiargrye.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gdashxmds.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gcvwegbeq.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/ginlyzzva.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gnjqmzzrc.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gecvxwltr.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/ggvhywiyg.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/goiemqbzd.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gwuwtahyg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/goytfznfy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gsmrtzjll.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gmtteywla.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gxbuseipn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gndrtlbdl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/ghuoxdbbe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/goekgbwgz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gqeoeovlu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gqmrmaffo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gimbnfjdr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/grnqmceqb.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gacditjco.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/ghgmezdft.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/ghpevgbiy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gqeoxmwun.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gmxgphiyq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gfrawnmyd.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gannmxvqk.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/ghocicrwk.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gkxkfyxxb.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/ghurhnxsh.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gakwutdjz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/giyppqjfn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gjnrrpmsi.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gmuytvsxm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/ghrnzerue.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gtnykjynp.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gwduabklt.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gdqpxngkk.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gddakknjn.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gkluidkff.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gbkkxdykc.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gcixdgpat.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/ggkafmgel.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gpiaeuedn.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gkuznswxn.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gobtvnjqf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gemhilvrn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gayerggpb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/ggncsbguu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gmwupilki.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gshcvtobm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gnwrwviom.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gzxwszuxv.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gfmtbnluy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/ggfhkqygl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/giuejeung.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gxnqtqcwq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/genorjhlu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/grrekxdbr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gtqxvavnp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/godjwuzxd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/ghksofpdw.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gzwkaumgs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/govejhjki.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gqzqkgxjd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gkplthwir.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/glmmxcbdz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/ggxgipngj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gwxngnxpz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gfnpzrlno.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpraewgpx.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gorgxfnvm.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gglmherpu.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/ggphwifrw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gpkjeiqlg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gqvkzpzqo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gjfpivtyf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gdeyescvc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gfmsgxkzh.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gdgojhulr.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gvsmkgwpf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gqdovxfty.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gvlaahzhp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/goegnwoyw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gdsgabfir.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gpllppaxe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gzyengifz.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gagxalztl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gimpezmof.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gkooagmhb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gnbrbujqi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gwpottfhy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gtwftxrxx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gxaugefiw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/ggmbverqq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gnslfrpng.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gjbbvcsvh.sHtML


<!-- 参考信息 -->