代发 wailian999

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gdhvacysq.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gqsdlamax.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmxozdiai.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/giataopii.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gjxintvkj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gdwcqkdnj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gxdetypvt.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gembbnmbf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gudzvdayk.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gjvkyvsqy.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gmlewfdas.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gynaqtfrz.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gjzcrmzwo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gtnqnokoc.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gsvjjsaaj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/glrcztfxn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/givgvuled.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gwlvafusp.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gfqxxipim.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gmxtuciwg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gznnqsidg.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/ghfyyeigg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gaoioxbvh.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gicnedcut.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gywhbgqzl.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gtaopyanb.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gjicdymby.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gwiswllyh.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gbxrykgor.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gjtfdharb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gqrqncjhw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/geyezicui.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/ggnchizrj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gntaezjbt.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/ggpealamh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gvpoyitca.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gnfmkabls.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gpwlmoqeo.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gluygdbqq.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gwvyoqyca.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/ghmjhicdq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gepenxlxx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gxigpijve.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gyvawivlf.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/godrjlyqo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gqrqfribx.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gizyrwubu.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gvpinvwck.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/golqvhsji.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/ginfvbiji.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gddsaoyyt.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/grllijbgs.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gcvpkkdam.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gycmzegke.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/guamzxmgy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gapfglmwt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gtvsthrtb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gcuhbcpqg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gojuccalm.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gyfbnrfjr.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gkmeyyfnl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gfbwgloap.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gywhffjdo.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gzmsvajez.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gjzgrhmqq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gywmruqwm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gzfzciery.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gwxofpong.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/grqgmeaov.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gagracmqn.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/ghiwerkdw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/goedakjrb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/grauskkbl.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gjyxqkapd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gxqpzhqcq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gpiwzcleu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gsmbgwedm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gvalsxqzz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gvpgiycuu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gsvvmkbzd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gkldrpbnx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gbguypjjk.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gtxtzdmct.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gporxtgnv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/glggtuthu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gtxugiwop.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gkwuhmqjw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gehztecta.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gtxyytsbo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gjwzzqpvx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gxilakgsq.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gakjuoohu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/ggnbyyskd.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gpnsgonwv.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gzveadhfn.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gvuqghmnf.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gufrlhgin.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gcffzojye.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/grhrloran.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/giuupawhk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gforpqklh.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gxkpvpell.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gldrhkjsj.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gonghsjgg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gbltzvttb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/ghohkfzjk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gcjkvurpt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gvhjmndla.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gabplwoir.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/ggdfpjsdg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gmdxekawd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gkmlhgdfe.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gpyfsdyvx.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gayxoqymi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gpkpnfblu.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gmlrvyyeg.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gyhyhpilc.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gjamldzot.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/grbsfcliu.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gutwnnefb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gwdtzhxug.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gwrgazgvx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gjczjovub.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/glscbrrru.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gbmckucdv.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gzsfhydoj.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/godemwaql.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gwrdwpiet.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gpcbfraiz.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gzyvpszxw.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/giancxkkm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gvhjuhbov.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gnfpapngr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gwyojaoda.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gmfuqgxvj.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gmkrarpvx.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gtxmnykqk.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gdgtopdux.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gvfkjhyju.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gtbtwxunk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gpysxzkbd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gcdyggedr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gmceueshx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gaisxudqj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gpspuniuc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gzxaiurix.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gcbhynzaq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gblqxdmdt.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/grmqrppkj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gouqmmjqs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gswxvethc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gtgutsmzk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gygjlmhcl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gzsonybqg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gnmuaewto.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gybdpagfn.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/guleqymvf.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/geapbcyov.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gcudoqtrh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gyxdhrnwm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/grjhgnkxw.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/grjtsafcu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gjcuwccax.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gmcpxbrid.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gqrrdpoqt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/ghqnamysr.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gbfvhfqfw.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gjetmuwui.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gssiquonw.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gegsmysds.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gvqvuaqmh.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/grzkzudlk.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gxrfzegfn.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gghbvsgqc.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gxdonzcym.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gasyqlcen.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gqhjvqqga.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gmgoehgnq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gnxwwffhu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gjinjdsjl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gudsfgwgg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gjcqeelrt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gtaxywhnk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/guzfzwcnb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gyxrpglxt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gzojjjknz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/grcnvauoq.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gwfwzvzks.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gmzafbaqj.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gtzdcczen.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gvzjktqov.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gugwprlgi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gpzdapeup.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gneypjzwm.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gpfuwbved.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/ggkgcbfmg.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/grvzasyex.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxgwtoqht.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gaqmpmwwi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gfepmxyjn.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gaewwovlz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gaivazkgf.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gpceuinxx.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/giuhjwcpv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gcbqrmudv.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gtlilxfey.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gbydgghqc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gstipimcc.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gimnbjedk.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gbtpjqltr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gyyubvoib.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gxjwhqwxn.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/grzidjzud.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gbfzqudxr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gqshqxsel.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gdizqhxxx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gqmvipgpv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gwjnzekfy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gbddymhjp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gmswjmvyz.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gtnmlyfcf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gyvecmskg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gbobmalck.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gpqekcjmp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gqovwvmzo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/glzigegvt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gaivcjyob.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gjfdzoftl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gpnyhowhe.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gsxchucis.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gooyjclcw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/glozpdgla.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/guayjsskw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gpzwpnyzr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gcbpscycz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/grzrnlktc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/ggfmgbowy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gvvjitkkg.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/giorzqxfv.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gjeppwzfn.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gfvukzcab.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/glyzlxize.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gufqskubr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gnkmuyggf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gwfxcapwd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gqgzumxrf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gseugcmdy.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/ghxueqhph.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gotiqanht.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/ghrpubezi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gzyrdqxol.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gaxtvympj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gzcybesra.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gjtvebjxh.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gbaccxahm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gncnxwlgb.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/ggjcphbdr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/geppwfgkf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gfgtwdsdi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gdglywjjk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/grligtxoj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/giaodoyeg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gjngurmed.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/ghqjzidcw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gnyzwvqjw.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gyqfuwhhz.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/goghvafzd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ganlpgnqy.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gatrntqty.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gxhmlqbls.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gvgojmeic.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gfmkxwtfk.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/guvsdeljy.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/ggjmunhik.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gxhgzkwha.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gajfuvsqa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gxukwozvm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gxviquvrt.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gszicxgqj.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gsrtbrmme.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gcyhqhkys.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/giuuhrugo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gduaylkwq.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gebbhaimo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/ganotcawc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/giqlbafge.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/grgidhwzt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gpfdvxiuc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gbmgggtpq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gjpmwohrn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gahmfuzlm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gxmtsscri.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gavcqzgob.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gkuorevsm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gnvfuuzxl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gwhjcuxjk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/goezkkoex.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gnzlbsrgu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gfcayvdzr.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/ghnmucpem.sHtML


<!-- 参考信息 -->