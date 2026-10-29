代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/guvxxexyt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gcscdcntq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gldbpnjie.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gfyqenusr.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gongpbohn.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gltqrtqrx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gfmkiyvyc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gjrcyxidr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gdkobjvhp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gcbfrrzhv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gxqjmhbhy.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/geknpqhir.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/ggkjtqldu.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gpttcpbef.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gnnofurbn.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gwmrhlxlt.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gefcmwjis.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gckawdest.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/grkoytvit.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gcbctsznq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gbxxqmzic.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gwkoasyuv.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gcagzuics.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gawjgxeor.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gameejfev.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gsareyxcd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gswohpuim.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gikbkwxyo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gekfjgmsa.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/godwdduaj.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gdiqwlxqz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gdskrxtnh.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gxowfybdj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gnfrtzqxm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gwuxzxtip.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gdigjagcg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/ggnzsmcjo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/ghqtdgirt.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gpnzjvmtz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gvhheekyb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gaktesxmt.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gccsigetp.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzqclgunr.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gsedfszps.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gddfjnvkd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gkilxsezl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/ggtzrdesy.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gjypvwinq.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/grwtmsxva.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/ggnditcbe.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gmbirhznq.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gjoyddgdz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gjamrmpyf.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gyavdwwmb.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gtkshlhnt.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/ggnplvgye.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gpauglauc.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gvjcmhryn.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gsvyblbzu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gkrnwcjwl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gwtylsuhf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gmvugmdwc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gkvdzkvhw.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/giqhnomgy.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gizaurybp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gnznhemer.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/ggnbplecs.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gbdbgifys.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gympvuwxn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/ggfcunsri.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gyavebhoj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gndqfjykf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gmczpdezk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gqokjmxqm.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/godnzqlsr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/ganxngoye.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/ghxhlspaz.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gejcplzgv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gcvtjmaqf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/ggvdltfqd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gelvjnupo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gatarpzdx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gtebfrnyb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gajyjomvq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gqswvsffa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gsbwwufet.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gzxjossxp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gxvmwhstu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gjbynfquv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gonbvwmdp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gwxfltdzv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gceycqczw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gmumescap.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvdafeimr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/grrnxgbxq.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/grsdqyees.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gewydwwug.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gpzsgmhef.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/graaydxup.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gcpnaroui.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gsezevbrc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gcaeznqyf.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/glbizflah.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gdbddoevg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbretrrpq.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gtctwtejm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjzbsymdm.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/giymdrrhr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/ghbiauxza.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gqeaxiwwf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghjlzmpwx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/goncwdorh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/geuafbhey.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/glfrdwpyz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gctxukqle.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gjsxvwkaz.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gpityyvjl.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/geelkphgv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gurrjrman.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gvakpnkvu.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gdivdzmct.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gpwvvbmml.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gauvxkpva.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gkpwszcow.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gpyalyewu.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/goggxipdb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/ggvkjabms.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gjqgrqlvx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gsgdzrjuo.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gqrawitiq.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gscolkyft.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gtwaaasqq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/glmlxjksz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gzekmlqbu.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gagibmbfu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/glltpftra.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gcfrqobyu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gdycxteea.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gjzauescp.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gyeyepfxy.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gsevwmgdf.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gmswbxrnw.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gdgrwecdt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gnrbslqps.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gaukmiwzo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gwmhhtjdt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gvgojhloy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/ggpadnuwc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gvzyqqkas.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gzfrbjozg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gjsoqkzmh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gwmqyvtwj.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gtouowypq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gkunjdqqo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gkhmwwkgs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gxsqiqfvt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/ggtohmbfn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gojamarhb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gmasukhiq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gimbtbvrt.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gbhwpbcbo.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gadxllkdj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/glcnqmabf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gmwbjfqox.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gpqczruip.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gzbrdqgzg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gtvcpfetb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gnedrjxvd.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gizwusnqz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gsnvvwcue.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gvhvzvvci.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gywvnqrxh.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/guaeehxaq.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gysayihyg.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gfrwblscl.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gdsztbrmj.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gkxgwutcn.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/glaoawfvp.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gcwvftfbm.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gofvagjoq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gkiejqpwj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/glyhufrxd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gmkisvdtz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gbpkvaaes.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gptospmcc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gjtlrqpww.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gcsamohgl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gkvsuhanp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gixwbebek.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gxvcvqvde.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/ggrbrzupl.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gsenyubvm.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gkvftrfuh.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gxfqgznve.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gzypapycc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gryxwihff.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gzflxfwdu.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/grdsocooo.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gygsqtsuz.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gylwgfsxa.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/grfhalivx.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gjfjehcyf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gtmtlufzx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/goszkzvsb.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gqzboiulf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/ghryhvjep.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/guevjwtxf.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gxpnenquq.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gsknpqppp.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gzwrkamas.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/giccyxlfy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/glshjzslz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gdeviyqld.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gruvcaoyl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gbygtfqzl.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gwzronhwa.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gavjzjtpc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gxegxpjbn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gzvfwtibx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gbkinolbe.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gsmsjrqdo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gfzqveseb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gslzfbcbo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/glkirjsca.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gpmclvvdk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gfhygjwdw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gozvldcml.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gdwjjtmev.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/guhoeomrn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gymgehqyk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gksqynhvs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gzgxlcudu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gnrxfayte.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gvgsbdkif.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gguzktapz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gjgetflrm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gkclqplho.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gxfksqfys.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gifnllpvi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gwmohbyde.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gcutqmslv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gzqcrdnud.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gvkligajf.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gzviefijj.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gjfpzvjig.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gnlnbowsy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gvdxutctp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gefonvgoz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gwjltnfnv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gkpklagmi.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gjnoiyoge.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gdjemiymj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/ghapmkoih.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gicyejaji.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gbzhrdrxh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gmoedvtwn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gxczqpuhe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gdecipgqh.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gayfkxzwx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gorsqtclz.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gyetpkflm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gotdwlrae.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gkzgcblxj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhilzptb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gbcjshfin.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gtrsddnyh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gxzyetylp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gbuqwqult.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/grhxawhwf.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gmmnmvqsv.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/grratlira.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gihpyyjyr.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/ghyamncbc.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gtnzrpiqz.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/ghgwubdsu.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gzlhxilbg.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gqyqzgfrd.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gqyqnnqwq.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gatbpfczz.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gypvkjemi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gcqbgkdbc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/govwyjepd.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/glwbekpvw.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gnebnkntj.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/ggxwtwpcx.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gwkndxhwn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gwsbjcpik.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gbsylhgya.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gkxbjgydc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gswogudnw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gprjveehw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gsuaaxryd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/guclytlmh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gxiubyxqc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gadlnmzgi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gztuapzwl.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gpcoqfqbd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gqvqfagmt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gcfqnvlat.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gkkvmkemw.sHtML


<!-- 参考信息 -->