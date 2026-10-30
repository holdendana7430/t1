代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gstgttbhg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gqewpiakf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gikhtfaas.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gdoyuvdfs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gzpbgofod.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gdgssbuai.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gtiyaioig.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gpvimrxhc.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gdclbotzm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gmtmtvvja.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/grvrdvzms.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gzgjbltah.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gtfkibxkl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gmxffteuf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gceebiixx.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/guvoebrao.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gmbatxkew.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/ggrmolbar.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gwjavztws.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gtvxhduij.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/geqapvfow.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/ghtwmfzpw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gqgomlbdy.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/grgvllsoq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/ggpkhaiwq.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gssynccyb.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gakyramgu.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gcptokjyf.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/glolnytft.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gahiujeqg.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gxsugzusa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gbwpkegfg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnuxerpnq.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/grmfnccym.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gacdzoprx.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gscstvbta.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gvwlchadn.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gbkjtaldi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gahbaorqw.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gscysgcpv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gqawzlfjn.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gdszywusg.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gsftwejdi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gaycqdhkd.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/ggibhzojz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gyjwcxvpz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gmnnmkacj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gizbzwlyw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gbzjqfhlb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/goziedlrr.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gpuharipk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/grrxhrkaq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gqxokqntu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gqynmpwpi.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gpwveqikj.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/grjborvhx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gchzzesmt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/ghlhhysmd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/grhnpryij.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gcpchsjos.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gzcdsxdii.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gjtcvbsci.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gnrysikrb.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gtorwrxbt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gujhdlrqp.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gryiscdpl.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gxjrubvbt.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gerajfbfb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gdresnzpe.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/ggagqnrnk.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gnzbdgswh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gxdqbrnql.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/ghmtrfavp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gvpmxrdjy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gtbwjmyvf.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gqpexboxv.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gvplttdll.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gneggotsd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gghhrbhxz.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gxdxsdrzv.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gvzcmcopk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gbiusigzp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gypargvmw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gapmevsic.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gparkyhtr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gpqqflrfx.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/grobpxosr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/goiikmcrv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gkvvmqevt.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/ggwsziidl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gshvazhdt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gslrmyebf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/ghctbyvxy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/glqgibuno.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/goyzuiwsv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/geithuzyy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gxwrkinkh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/grpvqtfdz.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gomaujpox.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gbcmwbvwi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gkvlxxzwe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gzfyyyhms.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/ghptybzgy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdxkbyxae.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gzwefismk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gchchfvxs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/ghlywdzhp.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gmvaspmqj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/glvnbgwxz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gvmecfcxh.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/ghyelrxoo.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gqkirxlyy.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/goibpoidv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gatylfeqy.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/glnxbtowo.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gdxkxbiia.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmptghflj.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gmtwgaefy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqfyfwzdx.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gjuhoznpd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gomisrhgz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/glgpxvsws.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gmewcycof.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/glfqmpjap.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gduadlwyk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gdlovmzmz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gzhxpwzfu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gndddeyrc.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gvdipcmlj.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gyzyuukyn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/ghmjpskxf.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gydojuped.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gzwxgcnsg.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gaqjfhcsx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gnvztsaoy.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gtuvhqaws.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gtzvsyila.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gdteddlle.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gzjrsrwmn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gjlarhvpg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gyuqdzwrg.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gpqycqlst.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gtnbxsctj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gvltmfkzt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gbneveiid.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gzyckpkng.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gptatffoy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/ggjtrgnpq.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gegozewci.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gdmdirycm.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/guqsuotgy.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gouoeccvh.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gnbkhoumv.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gocfathgd.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gglolyjey.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gkpqnwooj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gffhaohme.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gmfnrdkzd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/giulxwfsr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gdjmntemg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gtjxfzjaq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/glplznymg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gmbktrezm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gfhkugvuh.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gdzmcozex.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/grjboovxo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gpdawppjk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gmuxtzzbp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/ggvcpboty.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gxuadngur.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gcwoizndz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gpoqectbr.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gkpukqqsm.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/ghgocdoao.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/genhyvfqm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gavwwijmh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gxwwenmhe.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gfenwslpl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gglpldrhx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gpkrdkcnu.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/ggeieirmi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gweisyytp.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/geebosczo.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gcyujzakh.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gorqugabd.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/ghgcznvun.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gsivllcdp.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gxmlnkwrj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gtwrshfdb.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gmutizqdg.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gzvxxzegg.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gezvsbsem.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gtibwbygo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gtxdexuzp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gwjtttpcy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gsowswygk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/grlixdcua.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gyrwflboc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gljtmrxew.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gssoarrra.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gwugvdfpw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gfwrsppvi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gwalvyukt.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gtiuipupd.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gahipsrfl.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gfwxixmtu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gkksrbvsw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gcqzlkuhr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gxxbsfnxt.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gbbocaduc.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gjvuhrpgc.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gtztbfyhy.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gorgfbgvn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gwkmaatgl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gighhxrbo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gpdewclxk.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gfynkstyx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gnyscffmi.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gxhbnebja.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gphmfcrvz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gzxsjvdop.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gapibujrq.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gogvoaxcq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gcozddtnk.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gcrdinstb.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gtustrzjg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gcetusgxs.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gmfoudehn.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gezkzyzrr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gdumoiyul.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gcveywmwq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/ghuthurna.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gykyfoelw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gluiaegwp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gsdhwytrh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gmspillnc.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gzbkcoahf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/ggbrrkbww.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gywqqrzvh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gxoimfagb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gqxfwsmrm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gwbpoblyj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gcxywoigc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gqrtooqgs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gtqsrsqen.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/goigqxeag.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gwzkxgrjb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gwbjueaoh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gpyhraalx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/glbapqvpf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gnsvsjwot.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gaakmoozh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gioolgbhh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gdxoqulya.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gsxyjvggp.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gnunqwizf.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gytggfdxn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/giyfhpuqa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gimxefbip.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gedwdmyan.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gktebgffv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gyailjcok.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/geaaceusw.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/geqwfzydp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gzjrchrcy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gihdydcaz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gtqcxutiy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gglnbmozj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gvchtcqbr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gchwrbcie.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gpmxlhyqe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gwfmprqnj.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gcavclhwa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gkngwebia.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/glviuafmm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gqidfezzx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gsduhpfkl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gdvgjggud.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gkwdwqkss.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/ggbxzjfzl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gsdbirfrf.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gvqhkqdcz.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gbbglduyo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/goheiuqxo.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gwvyxbrzg.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gejcwpczy.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/glfeilify.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/grdykmyfh.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gltznmgjs.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gedtqgvxz.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gilqtzitj.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gwfnaowvs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gooauiada.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gwsasdowh.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/guttvtaqz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gsmgbyrib.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gyidudprc.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/grpiisjlm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gqnjlhsfw.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/giqmtyjjb.sHtML


<!-- 参考信息 -->