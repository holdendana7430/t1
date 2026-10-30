代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/goymfpvkq.sHtML

Go:   // 手写循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gpysomyzn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gvgbtwrvw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnzlikab.sHtML

[D15] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gskcnrgsx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowxoidfv.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvazavhhh.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqebiplk.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosiwtmnh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fanxiaobao.xyz/Article/details/gsgubytfg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fanxiaobao.xyz/Article/details/gjamfcdjf.sHtML

Ruby: arr.uniq
来源：http://read.share.fanxiaobao.xyz/Article/details/gptxoownk.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gcwrubxmv.sHtML

[D16] 求和与平均值
来源：http://baike.fanxiaobao.xyz/Article/details/gcvpnxclp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmweurtgb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxbolkvo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gtomgbomr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gpzlwgply.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fanxiaobao.xyz/Article/details/gfbgvtbuu.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnumpsfw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyrtglfs.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fanxiaobao.xyz/Article/details/gisakkayh.sHtML

[D17] 最大值与最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gezmopekl.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gohdukcgf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjnrxghe.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gasxjchja.sHtML

TS:   Math.max(...arr);
来源：http://baike.fanxiaobao.xyz/Article/details/ghqddmdxa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwgesayq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyejewky.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxtnmbqy.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fanxiaobao.xyz/Article/details/gssyatucc.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fanxiaobao.xyz/Article/details/gqiaubxqw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzqfqfpy.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fanxiaobao.xyz/Article/details/gkhkvjsca.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzvigytv.sHtML

TS:   nested.flat();
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcuosxzf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gvaesmpoz.sHtML

Go:   // 手写双层循环
来源：http://baike.fanxiaobao.xyz/Article/details/gyggtaqbp.sHtML

Ruby: nested.flatten
来源：http://www.share.fanxiaobao.xyz/Article/details/gudfgqiah.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gghbfptce.sHtML

[D19] 按字段分组
来源：http://blog.fanxiaobao.xyz/Article/details/graozotts.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gsnwxiqub.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkwgsixu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnkmzpzz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gymyjmqmm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvaynrcf.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fanxiaobao.xyz/Article/details/gjqhoomna.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvwxbcbw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowjhtrzj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fanxiaobao.xyz/Article/details/gphnbycct.sHtML

Py:   Counter(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjvioxab.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzjaafsr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gaivbpkro.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fanxiaobao.xyz/Article/details/ginpjivoa.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygkykhgm.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonbotuuh.sHtML

Ruby: arr.tally
来源：http://blog.fanxiaobao.xyz/Article/details/gwhftkmgb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fanxiaobao.xyz/Article/details/gleywcfub.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fanxiaobao.xyz/Article/details/geiksihmf.sHtML

Py:   x in arr
来源：http://wap.fanxiaobao.xyz/Article/details/grdmvhhdd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkxtcuaf.sHtML

JS:   arr.includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gniqrersm.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewiiwhnp.sHtML

Java: list.contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvolxauw.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gpnxvuird.sHtML

Ruby: arr.include?(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gxjzeumpq.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guutzauwq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtywjtkle.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkxngbev.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvogztzq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtahrgzy.sHtML

TS:   [...arr];
来源：http://baike.fanxiaobao.xyz/Article/details/gfpshhnzd.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gxuicypla.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsdknzvw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fanxiaobao.xyz/Article/details/gsdfejhrs.sHtML

C#:   new List<int>(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gbhcmvyez.sHtML

[D23] reduce 累积计算
来源：http://wap.fanxiaobao.xyz/Article/details/gfmizjuqi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gytttteay.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gbpgizket.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkngqxqum.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaxpvlrn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyksudop.sHtML

Go:   // 手写循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdztyleg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkmwpxwp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fanxiaobao.xyz/Article/details/ghzfxwskt.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqxzanos.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmvxrkln.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gpdrheoyg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gwzllsrzx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gonnljibb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fanxiaobao.xyz/Article/details/gfftlsnap.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzhrppqd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvsevlow.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fanxiaobao.xyz/Article/details/gjkrwiicb.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpctpuaq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fanxiaobao.xyz/Article/details/gdilntycc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guogzeysk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmrqckgd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gutwllbee.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/grxdnhcnv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fanxiaobao.xyz/Article/details/ghhlgtyjw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaapaftpp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclhclzvb.sHtML

[D26] 数组转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gzysbnpjp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnrprhpx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapmbtjut.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhhgbqiw.sHtML

TS:   arr.join(", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gubijbxqx.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzboagjlb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcbybxph.sHtML

Ruby: arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gnvmgcnru.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fanxiaobao.xyz/Article/details/gbqypsoqq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gckjeyzeq.sHtML

E. 字符串处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gaezdbfcl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqknbfoch.sHtML

[E01] 拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdowvttqr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrrvuaal.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysehtbet.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/glskftrrp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gjibpbaxb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fanxiaobao.xyz/Article/details/gzleugxhn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gyvtviaba.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fanxiaobao.xyz/Article/details/garccnjoj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcexgsjlj.sHtML

[E02] 重复字符串
来源：http://blog.fanxiaobao.xyz/Article/details/giyczcnya.sHtML

Py:   "ab" * 3
来源：http://mobile.fanxiaobao.xyz/Article/details/gflpkugtc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gekvyjzvx.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gdufzuagq.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvhoaycb.sHtML

Java: "ab".repeat(3)
来源：http://3g.fanxiaobao.xyz/Article/details/ghbyezfbg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmagmxrfo.sHtML

Ruby: "ab" * 3
来源：http://blog.fanxiaobao.xyz/Article/details/glqluhtqi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fanxiaobao.xyz/Article/details/ghbhlhczn.sHtML

[E03] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlsfeait.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fanxiaobao.xyz/Article/details/gbamcevij.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/grmsbclfm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/glgjurouq.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudrihmov.sHtML

Java: s.substring(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/glsssgqyk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdgdvkwr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fanxiaobao.xyz/Article/details/gfaiivdrj.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjivicly.sHtML

[E04] 查找子串位置
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmvafybx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gwpefgojf.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuixjecr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fanxiaobao.xyz/Article/details/geocfmiep.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtsajyjb.sHtML

Java: s.indexOf("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gvezpqyps.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fanxiaobao.xyz/Article/details/gbxljgrqb.sHtML

Ruby: s.index("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszfohqgd.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/grfaucfnn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtisidwd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gxqooeemo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fanxiaobao.xyz/Article/details/gyvbssvdw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqpxlzeq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqszzrcj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqkbuijs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fanxiaobao.xyz/Article/details/gzagzccmq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gycxwnvwx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkrnoqpw.sHtML

[E06] 替换子串
来源：http://3g.fanxiaobao.xyz/Article/details/gtwgqijlq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdryydkf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gjxfkciws.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvskzjcwv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gqgglfvuo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuocnqlw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwjyariu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxtjztjb.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gkubrnimj.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvwukwnq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fanxiaobao.xyz/Article/details/getazengc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gdkenffmp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/guoghxiag.sHtML

TS:   s.split(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcoluxhg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhcabffo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwbikkfn.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fanxiaobao.xyz/Article/details/gucbrqodq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiqzalhp.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcsvjosu.sHtML

Py:   ",".join(items)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwlrnutd.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fanxiaobao.xyz/Article/details/glhpuilaf.sHtML

JS:   items.join(",")
来源：http://wap.fanxiaobao.xyz/Article/details/ggsakxjgw.sHtML

TS:   items.join(",")
来源：http://wap.fanxiaobao.xyz/Article/details/govpuhbaa.sHtML

Java: String.join(",", items)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnnvclwa.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fanxiaobao.xyz/Article/details/gjtnbgrzl.sHtML

Ruby: items.join(",")
来源：http://baike.fanxiaobao.xyz/Article/details/gvmajroul.sHtML

C#:   string.Join(",", items)
来源：http://3g.fanxiaobao.xyz/Article/details/ghhcvnjpv.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grohmezll.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gszwssemd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaagaaua.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloljptzm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdglmiqo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fanxiaobao.xyz/Article/details/gvzssflev.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhgbsmtw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfbnfgyw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fanxiaobao.xyz/Article/details/gbqrvsjle.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbkljdkc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/guxklwxyc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggefmbeea.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqvsjbyp.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glndtgfar.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvrujsix.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/ggfudgicl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gntvqltmn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fanxiaobao.xyz/Article/details/gouryfccv.sHtML

[E11] 反转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ggajtbhgq.sHtML

Py:   s[::-1]
来源：http://blog.fanxiaobao.xyz/Article/details/gcwickrro.sHtML

PHP:  strrev($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/glaoicsml.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpagdeboo.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gwwklvqhn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnhgnlsb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fanxiaobao.xyz/Article/details/gxpiutjfv.sHtML

Ruby: s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/goayukcgq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdgdylbb.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbinttli.sHtML

Py:   s.count("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gtsvdlquf.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fanxiaobao.xyz/Article/details/gvvohxcmq.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fanxiaobao.xyz/Article/details/gdnmakqqq.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gegurjodd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuecpuup.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsefymlr.sHtML

Ruby: s.count("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgsjkhkh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fanxiaobao.xyz/Article/details/gngxdwrxx.sHtML

[E13] 逐字符遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gxassqcmd.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fanxiaobao.xyz/Article/details/goylygazb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizjkhcbp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/goehgmrvp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/gdtptdkzx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/goldtkdhv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gxhwkolgh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fanxiaobao.xyz/Article/details/ghzwqxmfk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrcuqqoq.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fanxiaobao.xyz/Article/details/gdhapjrow.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpbedmcd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrctujci.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fanxiaobao.xyz/Article/details/gaggzvsxu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gvwfwudts.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/gzrtspnkp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtodkujx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fanxiaobao.xyz/Article/details/gdetrspkl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fanxiaobao.xyz/Article/details/gyxbcgkim.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fanxiaobao.xyz/Article/details/gyycjrvei.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwohdnibl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gouxavxus.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnagkszrq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlmvzpbf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganidegoz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgpmrlet.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfcvnmqu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gejzxsxjo.sHtML

[E16] 数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlmzkzlz.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/geifdqdiy.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgugrkro.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeqxnvlb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fanxiaobao.xyz/Article/details/gsarcrokn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gretoxzut.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibxgjooz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/glpxoglrr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gadclrznx.sHtML

[E17] 首字母大写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyxlrygd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsybezoqb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gakimnfjw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fanxiaobao.xyz/Article/details/ghynnwpxj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkidwuup.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fanxiaobao.xyz/Article/details/grujrqbct.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/gxqtuscrn.sHtML

Ruby: s.capitalize
来源：http://wap.fanxiaobao.xyz/Article/details/gtwaxogcy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwfgxxhi.sHtML

[E18] 模板占位符替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhcpfzde.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fanxiaobao.xyz/Article/details/goaaelbwy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gabkvfpey.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/goucofeuc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/geemgbflt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhobrcnu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gxadmejfs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fanxiaobao.xyz/Article/details/gxjiptksm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fanxiaobao.xyz/Article/details/gkgnyihrt.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdhnskau.sHtML

Py:   s.splitlines()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbmthzus.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytwjzcnh.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnkbxlsy.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gczafkwbl.sHtML

Java: s.lines().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxkesbcb.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gernauimf.sHtML

Ruby: s.lines
来源：http://read.share.fanxiaobao.xyz/Article/details/gqykzgosb.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnrubjuw.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpkbuelx.sHtML

Py:   if not s:
来源：http://3g.fanxiaobao.xyz/Article/details/gokvgtjrs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjryagwq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gflnyvcch.sHtML

TS:   if (s === "") {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdztufpbr.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gusrhlssp.sHtML

Go:   if s == "" {}
来源：http://3g.fanxiaobao.xyz/Article/details/gqcrhxrhr.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gautmzdfy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gazekyumd.sHtML

[E21] 超长截断加省略号
来源：http://baike.fanxiaobao.xyz/Article/details/gufydjzuh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fanxiaobao.xyz/Article/details/gqymevabd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gvdrjbrgy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gktgygvhe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbtehdgz.sHtML


<!-- 参考信息 -->