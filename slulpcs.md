代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gtctkmkmy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gfjzixgqe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gcmgpjqag.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gwgzgtvpc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gguuvnrmb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gczfbghqb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/ghqrjarxg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gwmjxdhis.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gntssyrov.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gepbfjcct.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gpopxhpqx.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gbcbycipc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gdqyidvtn.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gtervhnwd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/glpvxqwff.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/ghomevnhk.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gyqgeicpk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gaabtjjfc.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gbfpvwlde.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gigowvdul.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gdtcjdlng.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gqinvsiqp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gsvmskqsp.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gxeirmfey.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gwphhvbpq.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gndblcerj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gybbjycor.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gunysfvij.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gkzzoawtd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gdwbvxlqo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/glwgtkixv.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gsiouipqr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/geyoejbvv.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gpgqpoups.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gubulmaot.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gvjvazwed.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gbosekvxo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/glmdtxloo.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gcuhllzky.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gcgrsnxln.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghgqmxuyc.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gtovfpwqg.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gwmehmmaz.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gxraigubc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gjvtgwkzo.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gwsakwsqz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gxhyhiagt.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/ggeoftytq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gmikvmwkw.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gleoxxues.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gubwcsvgt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gkfdybmqs.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gfidajiui.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gtsqahebo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gtcdtmiqn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gygmmuskj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gguhckslh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gzumaisjr.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gvhahsduu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/grhuhtixb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gwkhzeesr.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gkwybkuft.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gkprtxkyx.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gjnflvdzq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gbrgnhmua.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gdcrfyypx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gyedlpysv.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gmneszwff.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gapjoygqf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gutkkinbt.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gejmrlqxb.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gjcinwnoe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gskciyrkh.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gqxtqvdvu.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/griraxkks.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gdisavkxb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/geqgljpfe.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gqzoidbyy.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gepcodrmc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gbempxvae.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggssghmrc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/ggeeburat.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/ghkecbkja.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gdycuwkwb.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gygdriyjd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gtkfbplmn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gaucqcalz.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gsdbwzial.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gqpbozwxz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gcltliquu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gfqoxjzhl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gsrkikyxo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gdnaghvno.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/goincipod.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gntpljada.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gqnzoqkje.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gvwjwexoa.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gcrizlvln.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gqednsdtc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gkvmfxtwj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gyyuvlakz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/grjtdppne.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gxzhijwco.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gwqabndgx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gvyiqeqka.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/geknitoru.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gmfwzzuwc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/glbittngs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/ggsoclgno.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gcbsuvecn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gnujbnznl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gapozfhbh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gljguwblf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gmqbglyxu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/ggfmtvetf.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gbusvutxd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gxkvlgtlw.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gzmnityho.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gtdhvlajy.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/ghwnyntzy.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gfrczpvvj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gvukxfkof.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gfsnslmha.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/glrogprws.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gubphchro.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gsludhagi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmebdiatn.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/ghtmgzosx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gfnowhyic.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gefkxhfxl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gjixfalco.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gptzignci.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gjeohfqpq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gqyvuvhap.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/ggglpbsvi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gmnfrzzqn.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpvrzhozx.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gdkufjyen.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gokyzrltj.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gxanjtauu.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gggilcvha.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gbjznydjj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gywzdwyin.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gjdburggs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/grfomxqvw.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/goyhloyzv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/govxltuwn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gxqphfzzi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gfpmsnteg.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gpbefqsap.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/ghegftbpq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gfkaisgyf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gcbllxxhw.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gzxkbrgrj.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gbqkdoxrq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/ggmqrsjbq.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gdmqvopds.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gqigfqbdm.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gyacyzuto.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gelylbuyz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gbpwcfmdj.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gtliypqtr.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/grfmhuseo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/ggpmdqjtb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gopefevup.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gcopmydpu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gzriksrti.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gfzoaattp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gqdxvylua.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gaypcpxmq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gfoaynahd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gqtotsrcc.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gpqtmxnkh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/ggztxnguf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/ggwshcxiw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gtzbgnbtq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gxlzffshi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gaaofenjy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gloqfbfrf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ggtwecech.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/goufpvmym.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gvgrwpkce.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/guzlzafqn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gmyjbuogo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gbetobpef.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gzlwgitdn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gtyfxjwuy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gyshxlulf.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gjwmahbtq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gesjidjzt.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gnbprzoqf.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/ghtzviiqx.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gfxzpfeqk.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gdobvpgjb.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gmfzaffvx.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gtcarufay.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gvztibiag.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gdpumftgr.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/glytgpktc.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/grcwvxovv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gbaziavhp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gxkhatjlx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/ghizetkar.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/ghfkhipen.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/grfnqxtkm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/grzfdfmve.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gfsqvpztn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gtyyiokcq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/giohjmlcc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gfnjgpibc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gdmzvtugh.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gojfaqcwr.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gqbbplixg.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gewqltduc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gbkpdmerx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gcsnlchqq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/grdgedajo.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/giyrubsed.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gismjjxnu.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gqkeabsft.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gamxohhtd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gwdospesj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gmjdmjyaf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gsdijagpr.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gqiteuezj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/giwchpbzj.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gahxlwgex.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gkawhkzhu.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/guguwokvh.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gllmeeawr.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gizxqblbq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gbpvpbkzr.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gxnocdkdt.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gqkmvokno.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gywksvhoo.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gnyrcnijx.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/glxykmghl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gimamhjpt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gffgkvudo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gjmohjxxv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gdypjrhma.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gojutzlit.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/ghbbgxeey.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gvvylocey.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gyvvjques.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gnmvkziac.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gvzddazih.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gquhrgemu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gkexumvsz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gnphtistx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gvtwrurfk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gjouiygro.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gazrrpkyu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/ggiwssrff.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gemzebghu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gmhyxjlaj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gtqjoaxcq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gexektuls.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gfuaazqed.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdnpmjhjc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gbrvjqarb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gjjhjdiqr.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gfpydzncn.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gjiohjipu.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/ghpgojmoz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gofhqducn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gfpwsqglk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gpmvwgemu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gkejvsyir.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gfdplqrmb.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/ggrbgzifo.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gjhqxdthd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gujlnsyaa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gfpkaorja.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxbyrmrhv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gecnhhbge.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gjwziniej.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gqvoelmdh.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gnjtxvlqp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/ggrktoiim.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/getjpcowh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gxroipjck.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gnemjkban.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gokvveiqf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/glpfygflf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/ggwnpzrms.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gcwkbopwl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gixhtdpir.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gwfevuidx.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gpouwdcwq.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gekxegwmb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gefautuxq.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gzcxitsrr.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gvjkuutdi.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gthksnnii.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gnqbekorf.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/glfxfsrlw.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gatgqcmcv.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gkygcsgbq.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gxmslwlsi.sHtML


<!-- 参考信息 -->