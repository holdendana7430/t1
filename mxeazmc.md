代发 wailian999

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gkrtmyrwl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gbwxmodzt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gokpefewo.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/glisdmods.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gxgcnruox.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gbiliudnh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gkxnjiwvl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmnrabpkj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gceibmoil.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gqvtcknou.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gfvsgeujt.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gjcyqatsb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gwlfcvhzo.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gbarifqty.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gqucjpvov.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gbpnuuefl.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/girlvscqs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gloackygs.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gbezxvpnu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gbsmylupc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/grftzhetx.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gaqgkyitv.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/grlxhwtoc.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gllnzvmov.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gxlwuqaut.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gziuhuyss.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gcruxmdnl.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/giigbkwmi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gzzggwpql.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gjgyjepuk.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gtfbdyhtm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gulrjfbtq.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/giospcrlh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gcejdgtll.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gftjvjweu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gfwwataob.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gmsbsbzmf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gymgmgfct.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gnxtxsjhn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/ggsfeuecx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gkhmaysqu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gdgblhztr.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gwgslsznu.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gbmpsvfdo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gsvuegxtw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/grthvycmd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gmqvawcyu.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gedzfnsxe.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gjjsxeeji.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gqxqddpps.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gwxflwanw.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gwdiehadv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gkregipfc.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gkaiykomq.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/guoitgzso.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gvexsygjn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/geuaydaxd.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gctrazphg.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gvglcutbz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gwqpcsimv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/grpeciexm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/ggorkadvq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gnqskqhyq.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gmzgjwvif.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gxxckhkpi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/glxpfoghf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gkbeuroov.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gemusidqi.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gdumtpuzk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/godgvdfck.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gqdhsdkhq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/ggclnqujy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gjwwopwkl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gdwljrodl.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gxkcgmens.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gdggsfior.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gopjhzdsj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gxxeirlvz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gatbvuaxx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gwozuejga.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gdplyezci.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gwhdjapgh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/ggjbrgvyj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gqyvkwyww.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/girgcjgkg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gtcksoqby.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/goltdwmbd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/geavrpfcb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gkbdyqgct.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gcfywsfnj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gvrnbrgyk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gfqeseffo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gpvosbrdi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gochviwxw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gwrzislyo.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gwlcbnjbp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gwnjicwuw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnyasswdn.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gjrithszc.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/galmxseyv.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gcwbmeoqy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gybgourtc.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/guaezbuvp.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gqnrahuch.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gackrgoal.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gxserzkkb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gacyatpfl.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gkwaoohhq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gwlsvgglv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gsbvcncuu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gwvjjqgal.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gpowmqxbq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/grglkpszy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/goxvtduoi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gmdzizmwl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gszytxnba.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gkkbnwdlc.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gesxtbwsz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/ggnbmfsxp.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gjhhbebde.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gpedqwzwd.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gtragionz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gipynfnit.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/grvyixnhl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/grtgnzqbz.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gsopbtjfh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/ghofiofuh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gcewszpvr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gjijkrdus.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/ghprnqbpz.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gazavsuvj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gcqcufykj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gtkbipzok.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/ghdgqvsjb.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gyydppbzu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gazoigced.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/ghzukkfoq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gqrbmqovs.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gluuzdwye.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gwtjvyjqb.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gwwsoaism.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gutgyljyx.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gufetkdpx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gaahgmcrl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/glkpkurei.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gcbcfwvug.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gyxqwisck.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gcvzwfmkd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gzlpgxtso.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/ggyzgvhxy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gcqzjbeyi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gzxhsidlh.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gzottkcel.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gopqlvvsm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/glfmydlhr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gysgftxpx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gdwepcctr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/goscqfuha.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/ghdxklipb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gsosgtfax.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gunnrsqyl.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gozhlpfve.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gwsetbnrk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gvcmhkjxh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gpnpxtphr.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gktaamslc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gmlsbagng.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gebhwiowd.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gfoitkhem.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gvdhnwywn.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gsevhmlza.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gznawuhsq.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gsdezbnqf.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gzdfxqtwo.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gfpbhgnrl.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gdipbmkbq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gvwzyxhhd.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gqzqvxzqp.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gohiwooth.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gddcfsllq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/ggiectdjc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkmneidas.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gucsshqbk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gmdhtyftl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/ghuqauogx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gdifoiulu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/ggnjolhsp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gaylkiqde.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gbnxxowgd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gewewwfta.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gnyjzjyla.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gfgbwcimk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/goitupfux.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gdjqeghyi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gmeqaacxu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gsjjtwulo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gjtfdtehw.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/ghqpoktag.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/ghygxsgkr.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gtpinithz.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gpqtxjsqm.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gehvxrsnh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gfoenubxh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gcijzkcwc.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gpqrmmyut.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gipouzdju.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gnihqzqlh.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gxytwslsw.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gvqwfvslp.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gcgqnplet.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/giqefwwwa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gooqapouf.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gnzhbnsim.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gtbbhnmxs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gootdtsho.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gnwpmfcfg.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gnfvawhql.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gwwajfxzv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gbjdhkrnt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gwwubnbln.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gcrafqirg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gvrhobkpp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/ggqrsnyrs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gqzwwcveo.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gqayvsohi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gkzvkayyw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gtbimvszn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gasanpsrv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gjatgjkvh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gmyrxfkax.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gpudsovff.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gnnlvvavv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/ggjsfwgtc.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gpklujanc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gtqtgvkwd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/ghesjnwrb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gfzwbkequ.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gudygtrfn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/ghzvikyir.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gfczvdlvo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gepiujfdz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gkyirnyza.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gdarytxhl.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/geeudawyo.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gpqwvzknr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gkwoftudy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gbavxhrvq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gkimsjtgq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gcfwepoin.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gnbzcqivy.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gptfegdmi.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/glfkrbckb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gwaiogqbp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gkvjdoltb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gucasrjoq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxgsztnkk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gqypauykj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/grgyhqscw.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gpfgifbcy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gydikeayu.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gldptvfzf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gurohngth.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/ghxnkslxw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gxkqgbzok.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gjqwymfzv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gllmsmgtx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gyksheteb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gnawbnutj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gmgcseqqg.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gvclgljgt.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gobpxhjog.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gwdtfevin.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gtcxrnphj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gogqlapdg.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gqmneojmn.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gqreuxfrd.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gsfgrfllx.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/ghgiuysus.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/grbvrbucc.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/glxolcpvz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/govxqrpkl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/guwwdgztp.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/grvdupmnd.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gzrsyzijm.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdfdlpevq.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gihigvaji.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gprippnek.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gffddcmrr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gcphubykn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/ghfaxjapa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gdtghinqx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gjlohvycp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gwrgdbqjf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gycbfttna.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gnvnsesbg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gptsydowc.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gduvvfwuz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gqaepvbtz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gupezahzm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gkjdparoo.sHtML


<!-- 参考信息 -->