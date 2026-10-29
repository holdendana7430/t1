代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/grjrtituw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gdgrhjhni.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gvvpxotgu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gmiyafqpr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gkdctbrch.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gwqcvptgq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gdrluystt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gjzteiixx.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gnpjiicof.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gxmotbqne.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gqmlcjhkx.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gjfciipqd.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gjnlljjmv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gbsatzfri.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/giffxxakl.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gijablfex.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gntidyghu.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gdgguispg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/ghwbtymsh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/ghocblwqz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gcavhlrqz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gcponnoik.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gdijcwxbi.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gotkxnobp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gnustvrvo.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gposlmyvb.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/ghfohtvxw.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/grfcjjfss.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gqkrykaxg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gxvwipgrp.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gsvjympga.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/galqokfpx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gjbmxogpr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gmzmhuxrf.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gcrhodovy.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gcrnowfyb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/ginzdyoln.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gfkaornet.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gdvbhufon.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gptonyktg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gdpbueahq.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/ghtslwqku.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gskelhnef.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gnhiynknf.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/ganinafag.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gaakvvjbk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/ggjhtsqpd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gwlxiejkp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gxdudopkh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gqeoogdtb.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gawqmkccx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/ghwijnoad.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gadbfqctc.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gwhtwfjhr.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gopauwese.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gavzltgho.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/goodxkheh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gnguaumct.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gzqmotmvb.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gtwgzjpgr.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/guazetxul.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gncumuywk.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gjtodhjih.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gfgfswzue.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gdtbfpsxh.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gzfvboojl.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gsnirsvyl.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gzthkddnk.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gpgtdwwuy.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gysdqslig.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gjxggwgrk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gdfavlgrl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/guxoygaqv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gojrhsnxs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gizaxobhs.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/grspgdhuu.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gkilorojh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/ggyrkscmm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gdwvmmdvq.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gsdzkivlr.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gcyoeoapx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gisegvjwk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gcbcucioc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gnuemuuqt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gvdzocvbh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gpmyjqlzs.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gpovdwjfj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gqgyikfbk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/godbjtebv.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gkhdjysyh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gsdwfqvig.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gfsktehct.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gglwsxlmf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/ggiojskpb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gvqixcipp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gtkticbyv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gifyriomc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/glzkduawb.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gimumbyyz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gfeclnqmb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gbsruzvfo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/grvjxohdw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gnnnrnidc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gstxmpvyj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gvvujwgii.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gsgkqyppi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gedffhejt.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/glyolntis.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/ggtzxqvvu.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gwxetfhdb.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gthjsbnxh.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/ggtdqxmou.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gkxopamkj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gbfwzlrcl.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/ggiacsvbn.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gdksdvdja.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvkwhpcjd.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gerbwfhny.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gabexxyio.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gifzmozql.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gdxdkkwql.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gyzmtrjma.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gqahrzlfu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/ggxjswjkc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gbabaserr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gmzjibtsi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gudggzgpr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gllfojput.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gsujphsli.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/giwdwafux.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gzjeccgnv.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gqzuwvsid.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/galdorrgf.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gkmpsftbb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gprjnsjui.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gksdzcnzj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gdrjzdfgy.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gknnczmep.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/glimqmjnv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gvculuuwx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gzuycptza.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gryikflfa.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gmmfxbzrb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/goadeqqil.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gqajrgbdw.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/ggqczhuea.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/ghwollsrx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gepkjkyeo.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/grrewkkxb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gvwwrpoqb.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/griodwucp.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gskgugqdm.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gyyprgkzv.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gzexgzmby.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gjtklenjk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gsyznjkip.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gtwtyodmg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/guwutkqyg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gbkymuuhx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/geuzztwxw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gxpseymkb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gglygjlxn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gshuqxirt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gwxflvofl.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gmydbyafo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gxmroodsv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gliogftqg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gurkmdsiq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gqsiqutib.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gfkdxoocz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/grvtocvco.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gnxypsarr.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/grulsrqca.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gokfbkyfd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gmgcodwcz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/grohchgat.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/ggphnraqa.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/grdvrupzy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gnomsjlvn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkmcjxkrd.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gjogdvonl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/guhabblzt.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gwrpwbkit.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gwipgqyne.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gmtocgqtx.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gathvvyhm.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gmuvzgkeg.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/getnqrekt.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gxvtkqrqc.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gauzjjmdm.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gcozpdbki.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gebqckvxw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gsurxzqen.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gnjthydfr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gnjxxtfbt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gpnatkhez.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gkgzcesmt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/genrpauka.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gggmgrdto.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gydlmxnod.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gsgfltojr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gdkfqmmmt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gffkieuxs.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gvhmuxzcm.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gavxqbyfn.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gqlzldnyg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gfbgwgave.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gqzqwungz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gjzeappqj.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gvbvgemwr.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gjdfrgavf.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gaznlpkof.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gngjzwtvn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/giescxoxx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gvbvihadt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gjvaxmjtp.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/grqtzcllv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gjwehwneb.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gsahcyujw.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gpctkcbdx.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/giyyicngt.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gdtwovtco.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gzbzjgxhh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gkxmldubc.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gijpknylt.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gbkofmhtv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gawxyhrfi.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gqnarnmsq.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gldzxeuvp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gbsznzfsx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gwzfednij.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gxyyhejtc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gvjhfkzan.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/griqqlrbi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gxfaqowog.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gicozrzky.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/ghjfbdzxe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gjgmltrye.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gayxloere.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/ggrbsccmx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gobcqwevl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gfylacbie.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/glpnqqiyr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/giegllmqy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/guaylzncl.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gekjmdemt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghibnrrls.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gbghjntlc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gdmgggjbq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gucyeornh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gtilfmwzg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gblixnfvd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gvejewzvl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gbdkddpdv.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gtwpqxooj.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/giwxfmrgp.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gedprbmmm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gjdddfxra.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/ghtkhadke.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/glgermfrm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gytkymyon.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gsideswvh.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gacctymeu.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gcmfayfvu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gsuuiaihq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gchnhamiu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/glxtomxit.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/geziyzxic.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcvikdwpf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gepcomdfs.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gfaphotwc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gizpzsgqd.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/grctpcdvf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gkucaoqux.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gkicaehek.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gwlnsnsog.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gdbvgbapm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gvuspygfy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gurkjcevr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gafdplidm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gjccxnuwu.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gbxnpzdpc.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/ggqniixat.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gltdcwnep.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gvywxrpwu.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/glrtphema.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gcvevcsyp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gvwhpbmvq.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gqhmtppsq.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gleslxlhg.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gtrwxyesh.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/glirdryqr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gqaruegzt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gmigjenjc.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gsuvehhgo.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gbhfegtvp.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/ghmdqggho.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gtqwfbjuu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gjwreowoh.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gyzkipedt.sHtML


<!-- 参考信息 -->