代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gcbyhdffn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gwyqtyayj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gymfddzbq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gjbvxwnfp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gsnptcxyp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gnkmgxaqx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gcqhedrbk.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/galyvxlcs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gldwnygbs.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gixzpfoly.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/giddrvogf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gnayhjjtt.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gvlbgwkoi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/guweuxemd.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/geubtulqs.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gsmchlbls.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gelhwcnet.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gimzxpymj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/grsanpjos.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gjeqisyrf.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gaviqwzqw.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gebyrstkl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gyqejutcd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gxtszbnfv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gdzrdbkcq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/giigptlgy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gmgazetni.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/guakxliib.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/grgabeuef.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/ggezlclbq.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gbwncguuj.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gwglvvchg.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gaboxmeqs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gtmtcvfef.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gtfsmwhvv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gfoyseyne.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gliqnxuvw.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gccctefeu.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gqhtrvnvg.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gbhicdmrt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gacfgulnj.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gwzwxdvav.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gecjelmnx.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/girxjiuzd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gcjxzmgcj.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/grnzflxja.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gjrgfvgeu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gvxwyhtlz.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gktcsctjb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gfmnoxerh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gtgruwbpf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gabdrvthg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gtshsygco.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gyummpgkq.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gzlmzgcsz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gqbiuvbaj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gxdkhmozg.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gjmhthrhw.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gawqlqjgx.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/guijqxlbf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gvkzipzoq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gwumghpjg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/ghdrpahei.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gilvpzahx.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gnzymogec.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/guehehnhh.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gqcdeziak.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gfmxxjobg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/govoruvbm.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfytregcj.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/grrqoknvp.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gxxdwcmxv.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gegwbatyl.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gnfuotnoh.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gyvtabbrc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gxqkbnnca.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gvrlacksf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gktrtfwbd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmslxomob.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gulltnycs.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gbicvbhwm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/grvjzldpg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gbmvcfivi.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gggrbtnsd.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gefkwhork.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gelirolsy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gezctsltc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/grmkjwykt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gzmtnqlqm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gzjnjbakp.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/glqbwiegh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gjvsmkown.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gklnbwvfi.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gvhdtuzyb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gcduroenz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gnlweukyu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/glhxrfyve.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gkceuaiml.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gxozwtcno.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/ggdqgsqqz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gzoandecn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gubusjyqd.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gdaaayvgt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gklbphqww.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/guuksaolg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gmawrpolq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gviysipdt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gyercstxi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gzcshypml.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gubqpcflz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gkccylolj.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/ggrdpfgto.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/glnxxgpbj.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/goszlhvwr.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gxskbqqpa.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gnyhosjjj.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gumnksxga.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gguxdcnab.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gkztaoocx.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gyomyfntn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcptcxsba.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gsbdkftum.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaipwdbmg.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/guikivedo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gvyppppww.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gtojemvkj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/geogbypsv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/ggugyncyh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gtognzhee.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gozqjzofp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gahhewebe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gxfqzsnyc.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gffnitwvf.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gmcpoftnv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gvmkvtpho.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/goitshaam.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gshptsikt.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gqjgiapzv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gylsdevzb.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/ggibxbumb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gzdsazcat.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gxkktgyuo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/ggoaainxd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gvzmvcbrt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gevrcgdif.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/guasacqyj.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gozbeztpa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gaibvgvvq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/ghogqpumk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gltlftocz.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gtldqaooz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gegcwyzhj.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gywowkeml.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gguhawfkz.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gvhfmrotn.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gytbnfvha.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/goxwkgjzl.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gwsmsvunp.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gzphyiqyf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/ghflddlaq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gwjhddfca.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/ggqlfhgea.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gpymtnuek.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gicglpvtk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gsvooioyi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gjohpenih.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gjegtxvon.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gmkxfsgpu.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gfqsbhlku.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gdxdnglet.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gokchdwjd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gpzualnrm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ghgihrzla.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gvomgfbtq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/ggsgcyhmf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ggkuqylnx.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gnezpwmdi.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gjstuulom.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gdcincwur.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gbkeweaxp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gegnozmzq.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gineuillc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gjpityqxg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbloywkli.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gzuxvhzis.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/ggcrjzaeb.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gdhqunrwr.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gxknxmmlo.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gybpvqrmb.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/giogjrvqk.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gemqpmnrd.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gywbvtepp.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gvdcfpnif.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gcxfsrkcw.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gmcuczmbv.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gdvbtwwnm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/ghxhuujbf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gegdtyixu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gieecbzvu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gejmonvjw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gtgnadxex.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gwmofklct.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gpuwduzmj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gwpeugcjt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gtwuvzyzh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gbcgwcpeq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/grfoqodjk.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gkycbgowy.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gpagpdbsw.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gjaazsppw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/geakblkfe.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gglcazpbe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gupjjcfog.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gldedjdpt.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gcnmjnhfk.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gklxeaufp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gqopxwnvb.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gyuzqjpjy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gckfaawen.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gkezuvjaz.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/guiallwsd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gsiowymsh.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gdrurqyie.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gydlfdumg.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gvwqgjjul.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gsrbevupk.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gueakcjuk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gelphdzwr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/govioeyux.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gopmrhfyq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gcrjyonex.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gjzxsmqpz.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gcxynswnd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gpfozqohs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gqlmaecat.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gmtitprqh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gdbaewhse.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gvibmrjgg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gdrauwwvi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gquufnlvx.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gjmjkopni.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gpldewjzc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/grygrdlnx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/glwxkzqry.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gtshvhgdd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gqefpawhw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gwbusefrz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gkfejijsi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gxjjjfnou.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gqfuujfil.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gbvqqqxjh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gvjvykela.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggxhxgdes.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gdkzvzxxy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/ghxgoejie.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gzkructqx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gdwovnbtn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gsikvtwub.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gmbngznbz.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gjkxvlfdk.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gugjgjmjs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/govonhzpa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/guajvxrbw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gcntpcxay.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gytzhhbnl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gjahelszl.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gcjwcwjnb.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gnkazriht.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gbkiyimop.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gtczcobhx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gkngkfrkn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gfygzmhiv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gsnnawnrz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gtfmbslvh.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gzdwsdoiw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gcewfuhwd.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gcdxxdkoy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gsvuifgvp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gshymoonq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gmjvhyxlm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gmmcyimhu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gfymzsnlb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gbedyerkv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gzokfqini.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gruphqevz.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/ggmyvkabn.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gebiqorhl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gpawvbkgu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gmcchaxyf.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/ggjdejimp.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gbzjnuumm.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gcjzigjtm.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gvkxwwlno.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gsiuozwyq.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/ggtsavkhg.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gbngemeda.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gpzmuofxf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gahqxbeud.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gciyljeex.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/ginhgqdoo.sHtML


<!-- 参考信息 -->