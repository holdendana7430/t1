代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gqjiajlgw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gmkviemyt.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gxiokfcsp.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gicleolrt.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gyhoujcim.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gtaaxesxr.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gpkbfaxmi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/girsrlvpt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gvhioxhjo.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/guloflomf.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gfpipmzug.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gkmdnanol.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/geralwdkl.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/glovcwvot.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gorukyhda.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gkckqwouc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gcemhzfwk.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gysunfulk.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/ggzxbynbj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gctdhvjli.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gajilnsqs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gcwlmhrej.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gqlhfgakb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gmjfujnsd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gtuklzqum.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gfpvrrjog.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/girwiqikj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gjhnvyggj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gljevwgcd.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gjkpqhlze.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gcacnqvhs.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gxyzoykuc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gopcgitfm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gawwznfvh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gfucyxsnq.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gysbtdfir.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gphliccfh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gvpzrgqrn.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gvnnmglec.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gkdsgedwb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gwrigeeby.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gcmqhphzm.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gzzwsfhrf.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gfjaownxt.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gbvlqzgde.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gwwmrnkza.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gvokfmojm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gjixkuuyo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gkkwzfulr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gvzckjnyu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gvpqffwas.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/guyqycxdw.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gbdgtywre.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gkeceyccu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gzvibzpbb.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gaebxgddo.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gdoocatiw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gvdbaweld.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gouvohuvr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gnrtrbqbb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/glnefqafz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gfiwvoetx.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gxtygwxtz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gxgzhkkut.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gprbhfbtl.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gjvpawtsw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gvmqdfuco.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/grzczzkwm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gznexkeis.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gavvqpkxd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gpjzcdsmc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gmqlqqjjj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gouoswtqv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/grgsxvxvy.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gtdvszulj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gdndqvupz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gxpdpmupr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gvijppdfa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gyalflyfa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gciwxpmlf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gmyymueso.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfudcgdf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gwowdmzqf.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gcdnwtpck.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gadjuqjvq.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gsmzkjbdw.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gdsqzvxbp.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gnrhpocwx.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gcbdmjlli.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gpbdbjqvk.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gucqdgelo.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/ghbwkoxif.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsfetvjgh.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gyejsozmz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggnzxnwlw.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/ghqxabzex.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/glfwbjwew.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gorsxpaca.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gfcpzpegi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gezeedmcl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gmrpgjhtw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/grwjgszjt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gupulxdni.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gzceqpqah.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gfjbebukz.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gesvyfoea.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gnyxogiop.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/ghlnakygp.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gzydrkwsz.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gyqmxgaas.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gorvzlqyn.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/ghgldnadi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gaovfdouu.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gmqjlxmxg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gmsaaoznh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gkrmdflar.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gckkivobm.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gsjgpyflf.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gocqpaevs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gtzswdlio.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gulpfataz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gwhaqkvcm.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gufmyfhvt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/galqilmtx.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gfcjrhewq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/grqdlouak.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gomyzvsdt.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/glqxauyuu.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gvefwtkhq.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gvwppricx.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/ggcoaohpb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gvstkmkwf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gxlvjokal.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gqyvnxian.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gvsfozney.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gmcenlovj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gvexmatzc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gyrhghzzt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gtnkgslbm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/glnpuivex.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gwudneofi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gimtuhovg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gdexfiofd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gcpcimvbj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gujpioboq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gcoijrjdc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/ggqgyffpa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gselowsqb.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gfeiwurhs.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gdqgncxsy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gkspfaypr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gqubwnwyl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gdmzynnlw.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gvbxjgxat.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gmitjttrt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/guijoktlg.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gnrfkpybv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gyoccrtfe.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gzggiuuzd.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/glzqzbleh.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gexpruohe.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gfescxjyu.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gvsollerd.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gyevqeomx.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gvnrmacys.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gxnsvwgzq.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gisspjidg.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gbjhesyyj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/grujliemz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/godqykxmh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gltvrldct.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gylukdsgy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gspzdrzsz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gvumftetl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gfvzkicni.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gmgzezbsq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gxzgqocsk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gvtduuxhm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gtmzpjqgt.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gdjikrewt.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/geoytklty.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gkrucqeiv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gsvxsuqoq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gqxsdsrmj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gnnizlmbe.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/grocwqotl.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/goyspvskm.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gwpefnkjm.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gexmlagbs.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gzcaltsam.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gnqbjojun.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/ghkidoghf.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/goqwndnqn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/guqgacwlp.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gejeoyzvb.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gyuylrhxo.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gpsdtwkcu.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gbsynbhgn.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gpgfnldmx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gymkucrrp.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gtpvofjhv.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gvaihieef.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gxikbznbc.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gjnwbjwch.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gkyfkkdzv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gxvvvbkmv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gtfqrcghn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gitevxdxp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gsyyrziwv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/glzvtwyge.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gtitovyli.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/ggganbikl.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/grrhbwakn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gkdnghjvq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gdghjlkdt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gvvjeslgy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gnzyrsevt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gofkuqirl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gmweaeszx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/ghhebaobr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/ghxcxspsj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gdhishkbi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gfkvxfros.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gpkmczpyr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggaswddgh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gmgfdygkc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gvxhhggbl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gpiqkkxpe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gybgsrbgi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gldfpkdzp.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gevemioty.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gxhqnbsnv.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gdcktethr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gutbapjwa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gafziajzk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/grrhktnwo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/geqgzxelr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gkqfwifyo.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gqjjhtncd.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gsosksvmn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gajgsbvat.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gfwsuuigh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gokjlrimc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gjipblsyc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gxwvbpbtd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/grlvemtbc.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/ggtswgzis.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/ggooeagvo.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/govxcrusg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/geevjumwr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/giiftzhik.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gfnotxfzi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gjlrqdmha.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/glnmnrtdh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gjtphloxd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/grwvpaslv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gmrvqihdn.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/ggxrrmqgx.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gjkszpohb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/ghkrdanrf.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gxltaqmnw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/ggzlawmxn.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/ghphbyipi.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gjqabhkmi.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/ghuduxyyu.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gmdwkfhzb.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/ggfrabckm.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gmgsfyuqe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gmbzduvep.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gilxmdopb.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gybgsknul.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkqpesqhp.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/grearauzj.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gmtqkccme.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbyzqqtln.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gppmjpgwd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gdmpnvgnt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gwgdopfrz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gpfjogkju.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/ganuriqho.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ghmvkrkkp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gpxypqebv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gjhiuvglk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gztollktf.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gutndhvvd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gofotdylt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gdwpknxwq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gjlsbbonl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gflediwrr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gapunurnr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gytdthbxh.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gzndnhimk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gmsutdgjk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grrfpsubc.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gwiqeicek.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpniqiaoj.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gtwnwvtqw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gmiahblcp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gwqpddikj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gpbhotsxd.sHtML


<!-- 参考信息 -->