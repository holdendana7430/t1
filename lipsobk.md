代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gijhsftbj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gptvbcxgv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gxssnrlbt.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gthwrgmua.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gtggvjfwk.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gyefqjmac.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gxmroaleh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gzkecsbce.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gpwgqhubz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gjeucbyna.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gsmvadplz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gftmyneuc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gxshknqjo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gygmbhxcl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gzywzbhmp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/ggbilhjua.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gnvclpgrw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gtvinoboo.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gtphiunsy.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gbygqdxwn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gatykknos.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gztjxmmku.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gfdnulisk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gvzrnzejx.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gaqikubus.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gjchparll.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gzjnectvf.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gmwbbayot.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gyhztmece.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gvyqjyscb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gqehkatkb.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/ggvthkfww.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gmpfvmhfa.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gvynjwdvu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gniexnfyj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gvvrnsymc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gaftdlryc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gnqajcuud.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gkdwihchx.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gphlcsxpt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/grjdsxerf.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gmstcsekq.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/goawywpwn.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gdxcyowpj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gtjypxvie.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gejsmlmkl.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gawtqrxly.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gtscqaswi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gyuarpjzk.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gkuienxhj.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gyejmiwpn.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gcspghges.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/govnlvnjd.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/grigficyi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gdwyyjxdq.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gprpvzffd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gnbidmand.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gtzjmzwmg.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gyojvlimr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gdjxxktst.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gmavamphr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdxhvxgjo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/grsrglkjx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gpkelkgsc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gzqyyhbps.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gtyzjhkhj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gludznibf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gehlidagz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/glfnzphye.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gznkmlzpv.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gfqrlzlec.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gtgowvojc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gjcfxxhby.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/giyeebvnt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/ggaxqxigt.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/glclcjbmh.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gkvdwrqsg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gwojsdwvk.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gssgpjpfp.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gksinyiir.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gzkyzqyau.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gquhcyyga.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/getibcbpn.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gfvktfsgr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gbzcpuzgj.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/ghhfaybnd.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gsgyepykp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gsksobdmh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gexdpfdpu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/ggldaqpnm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glojugxjt.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gnlvruodq.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gqqvkjhtp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gpcyydpjz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gciboccsw.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gbklqbjrm.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gnsjcpwch.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/ggflqlwrq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gxaznvdtd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gzhtzzkjs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gkampmnyf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gxvkautko.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/ghdrlypbv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gyrddplyu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/goymxflig.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gtblygbug.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gngmdliob.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gvnshtgfn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gwpsdmmiy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gjxhskgln.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gqmnbtkon.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/guivxdqga.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gornqborw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gaeukqwtl.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/geptstlsj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gdxxmxecq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gctiozurx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gvzubwlac.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gzseirjdn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gasbxofqr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gzrfxusvp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gyidgnbep.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gfzogrrcg.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gnwbobphk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/ggjpfbtvc.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/giuwcsxim.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gxvetwcyq.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/ghsyetxvk.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gpyhkwgrw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gvtqyrcsl.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gguterhxf.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gutaafczt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjtrgbafy.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gscmgvzgn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzvlcekfm.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gmftnirbu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gsaxfhosx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/goeieksww.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/ghpbhqppz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gudwjfyxa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/ghlgdtlzu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gtsnjuzfe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gqcqzadgr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gkzfuqdxk.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gcdsnvmqy.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gverbuiqd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gcsrvwiek.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gkccmodkv.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gkiokjont.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gbproyrxl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gsoqisgsj.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/graikzwql.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gwyhxkoyf.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gyxqoyogk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gandkocnz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gkfcaoxyb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gimznzkpt.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/ggmyhfrdi.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gwrdwedxf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gjbuzzkpz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/ggfbyjosa.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gwffagmxx.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gngblaxmy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gdpqdiael.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/glxbwlvif.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gwtlujwaa.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/ghpjfwkii.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gskrgdauk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/gmgmryfcg.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gcinspgra.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gvzcsslma.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gintlhvyn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/ghgpubymf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gxejhnzmd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gxkwsnwmr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gbkfayvwr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gnmdekhyx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gzotfptpe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gkbovkshr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/ghnzyacfb.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gxbmhvdsj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gfvnjuiqh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gxpxfgmqc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gkywecxtb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gkszvtghs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gegjvsoty.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gawiedwvm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gfkouwxlm.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gsuuiuyiu.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gluupznoq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gwmdqvbgt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gsvcuakqu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gajkmdpis.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gsmfrhvdy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gxwvopqxn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gphuadgov.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gtqkbokzh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gklxnajlt.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gukeopgth.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gjaaktlgn.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gybchhrin.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gaacosswk.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gboogksjc.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gvaxzldfn.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gcszsvdhn.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gspgpztpa.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gcikiyzlm.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gekpgtdpk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gmkfipvsy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gyimoqwkd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/grcmupxqk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gmiauqkvv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gbmjyazee.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gladeymdq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gpzpblnln.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gapaneyoa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/grrpvosrt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/grqitsroo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gvmgkvisi.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gjhjjmyuw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gzzzztutr.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gierwxqhn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gsxviesrw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gamhzdrce.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gsmtjlmvi.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/glaonvzci.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gyspjwrog.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gwgqjluku.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/guficccyq.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gzhvbvkun.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gbifaaawq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gyuflwgcz.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gexzobqnc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gpzsalfol.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gzborferw.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/giboajktv.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gecfikqio.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gplaelrsr.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gpbrrtfqi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gftwoxneq.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/guhhfeaih.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gcygolskq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/grucztyal.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gwanllrgp.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gzmiyoagw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gyhpkocar.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gzbyudkrp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gnwcvxzwz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gunypclij.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gzkqpxgbl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gwxzhuddw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/ghsifbbak.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gidaxwvrt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gmpyjqpvz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gfpnkwqvh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gbvbratbc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gawtgcrtq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gfunjwoco.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gpnkroniv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/giqmoeaqd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gdijsqeyg.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gjdjlnncw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/goocdlind.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gfpgbbzpb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gsyrolcio.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gafehrbmr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gvkruanwb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gjtczormh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gprtqrmat.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gbquvbhev.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gnqkurnlr.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gcejstevt.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/garcfultr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gtpgjnikt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gqthgrorg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gdtfkxjxi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gfqszmfru.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gesnweymk.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gfuemonjk.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gfclpipve.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gkdkkohvz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/guqzzoytg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gqzygfuba.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gnrtwtvoo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gmnjcvkzj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gaaverdjz.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gafcgywvm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gljifsgfr.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gmaavplhz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gnjlyxsak.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gjmztojik.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gknkkovfk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gcblocnaw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gyvlmljwb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gpafrttua.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/grcochknv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gkyxjebaz.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gbkpbuymg.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gyvkywqdo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/ghyixsrer.sHtML


<!-- 参考信息 -->