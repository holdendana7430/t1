代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gdgoitcfi.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gcgrhrqni.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gxtpstcbz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gvvxmnvve.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gnaszgiwo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gnuxwkimx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/ggfnxrgdx.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gayhfjwwo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gpophbefd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gharykdsy.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gdfdvvdwv.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/ggqrznnjv.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gkcjkpgpq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/grjafxrcp.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/geavxybxc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/giyrwvznt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glkxigpnm.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/ghnugetjz.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gnfvodfty.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gsrkspsuu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gtmwgnmeb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/ghbqpwger.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gbngwgkhf.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gymthpwvq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gqxnyskmj.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gevmobwpr.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/goegumzwl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gobapaspn.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gjrbtjpfa.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gydomxihm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gtvmnkcea.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gxifxlsck.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gemnroevx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gbizsgmfk.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/grxvvfsaa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/goxbfzacs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gabohitfy.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gjqupnhfs.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/ghccgzbzm.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqpyyyeux.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gqvuwtzuw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gylxrcsbs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gnqoullss.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/ghnzrywxw.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gwsquzvjo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gathwofya.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gztkozrrs.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gltocnxrs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gkanfotbc.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/ggtvoytca.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gzpbowxpe.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gasbvjwbz.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gxlmruhhh.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gggfhllfu.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/ghoaoibxi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gyahyytea.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gyatwotwi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gtzhwgwyp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghdwmjyvf.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/giugfyttv.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gviuhwfeu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/ghhltpmlm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/ggoqfokju.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/ghljkorxr.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gtmlmpzpc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gmsyjdieb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gzblfdjht.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gizianrxn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gksaimdiw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gquucbrhe.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gqwfgovwg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/giuspfoif.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gaxrjnchb.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gqglanbbm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/grhzueisa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gsmjgafze.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtnztnzpt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gtxtwxmml.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/ghovgxiqb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/godxuener.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gotrounpq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gbxxgvuwu.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gerpdbrup.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gmvsykdsg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/grqmduvrm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/ghyfgtlhs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gdcttotan.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gmbckvmxw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gsrcvszpo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gltneakzn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gczugizrp.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/glrplfcck.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gikswwktm.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gehwfsjln.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gstbuluvo.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gczshtwqv.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gzinopwlw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gegmulcpg.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gtwfcsdsc.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gpzgntlhz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/giomkrmof.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/glocpwspq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvbdxnqdx.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gfnopvfmv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gpbizmscj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gjpksyyjc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gzlhtlhrk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gbnbbzrtz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gtvnbyusn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gdzvpymww.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gmxrfmoyg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/grohbrpia.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gdtnkiugs.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gvkovsvwi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/grckxxupr.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gjdxyrecb.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gscupyquu.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gxvoipmkm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gqqcckpgu.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gsjuamrdv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gisdndjsd.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gqwspxogj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gszbmfkff.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gonkscymw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gjmoxbjan.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gsgtatrwo.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/guekporwz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/ggrzkqynn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gsdwkmgyk.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gkjpjttfx.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gnojjxnhm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gcsujjlpl.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gxbztituj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gqzeymsdr.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gohwdnrkp.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gdsuphksm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gpvanzkmv.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gkrvczuui.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gfmcsjomu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gjbdhapid.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gpvssvqdq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gyeqrbgyl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gkgzcvsmc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/geimvcbxl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gixcsadam.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gagzszydo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gwbtxzuwl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/glvssidgq.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gktjzcwqz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gqbxlhezm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gsfnfdnnp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/giqpcmbue.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/glugnxkrb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gvmmudwga.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gxeriqhww.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/garfasckt.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/ghlavpzbo.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gkbmjhyxn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gumicfhur.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/glunkihzq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/godvumeyk.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gejbscjpe.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/glahnxggt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdozzqobe.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/grfrwlmwp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gohrzbxrg.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gvbindxxj.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gracmgtes.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/glhjqdlju.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gxqvytckz.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/ghswdbumg.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gdeaculwy.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gidfywmoo.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gdfcpqqgt.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gkfkgneyd.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gdeeipmio.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gjktxclby.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gvsouvaac.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gkejcqkpg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gapnxllqd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gxelusbxz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gwckkkarc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gzlbykmtl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gkvylgshe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/glfuuetej.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gfivbmmxr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gbbpylseg.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gasiufxup.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gpxwfzlxp.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gvhlrkadd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gimwhrhrd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/grlpsueks.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gouolfood.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/goagsgset.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gedsdneuq.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gupqtuquu.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/giruvqtsk.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gkmkfocic.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gfblsapqg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gjbtizpbd.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gdqnutfyg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gvmemundz.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gigtuvxdf.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gprrxuqnz.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gyokrksuv.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gvtpcgkrh.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gmuwktlzt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/geqrepyfg.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/ghnaejafc.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gfwsuogqp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gaxyduyek.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gndtsounp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gphraimyk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gprzvkwwl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/goxzerxqe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gdptaoptu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gfhbzqudt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gvsmwzvxb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gvcmchrwp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gzpjdmsmj.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gbasztthc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/grajpziok.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/ghkzdsnns.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gmigznwjq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gynwjdhnw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gkhigbjxi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gxpycmeul.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gmirzxqyw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gdsidjjgr.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gnyceloob.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gwytdwhxt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/ggkxoopqm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gbgalngro.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gezwgvrja.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gulbokroy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzankqyva.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gwcyxjvls.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gclofpizj.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gnpixmerc.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gtngmelfa.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gfuzplyyd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gsbiztawr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/guztlyfia.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gpachyqbp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gehkqyqvk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gxhfbbgkp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/glgiiycyb.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gjriqjrzt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gfckgsqxv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gwbvkopjw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/grygugjrj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/grpgcloet.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxcfbmubm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gsauljkwi.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gtdggcoqh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gkenhgqzs.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gekczrpjp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gfmtzgzid.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/givicyqlf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gmlfcvmkn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gdayljvkg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gkskzefqc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gwmllfkwq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gfentiowd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/ghvpswjhq.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gjifnvhxo.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gojlmdrtx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/ggfcckjjm.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gfofdunjy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gprkywjcc.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/ggwzgeyct.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gklkwrgcq.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gwjynfzeo.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gegwyfrtt.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/ggereprih.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gveyoqtyd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gbwczbyju.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggewctabz.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gkcudnxbb.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gscshfbeh.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gkoqmuynt.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gjgngaykg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gtiolhann.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gdfpkxckn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gbcvtpphl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gbggykpxa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gitnfujzb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gmcauuxrf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gyyddsizl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/ggbqgibav.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gkrknzxxf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gsdnmwssx.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gvlqiczwy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gdsrybqkq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/garsesfjo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gfgbfbish.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gluscckea.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/githwyfls.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gskezmqhb.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gipbljtmm.sHtML


<!-- 参考信息 -->