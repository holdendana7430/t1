代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gzdqqesrm.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gvezvqonk.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gxrkrbcoe.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gxjlcpqkh.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/ggiqahdwr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gojyelcwq.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gekuuqxvr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/ggujjsnxg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwbmcczue.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gqzpicxla.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gdlkwayjt.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gtxqzjryv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gjpxkvgjn.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gumjhkblo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gumicaivf.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gpeyetcpv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gplcdqukl.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gmguxwgps.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/ggkbjdnhr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gugtiqzrw.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gqldutyss.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gcyusdodk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gtcyxztnm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/glmqxpvat.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gxfnifwyl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gjeeiyexw.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gstcriukn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gjqicauxj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gapgpjzef.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gkkjzfpxf.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gkialbnfu.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gdvdvbbvn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/grsdzrjag.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/ggzkgtdiz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/grprugmob.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gtigppnds.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/goyotsoep.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gchjhpyez.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/grwaiyglq.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/golhghqcf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gcmacnizr.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gfmshqyqr.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gyswgylza.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gbpyuxieq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gjwqmzdeh.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gfriqpdwo.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gyhklngkz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gtzkuzmnw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/guecttwog.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gjkogziwu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzivrijkm.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/ghxmzufkj.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gqjlcjvbc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gkvwaxces.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gljutruqa.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/guqrnyitt.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/ghciwaekr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gdhnngzha.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gmpazcfvv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gbmsodong.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gziwnqmln.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gpjnmzjhb.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gciyaouni.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/grwjhmxsl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gjowagmtx.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gaeubvkqe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gpmedgstn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/goadjsbdz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gklxgqdxw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gyfhhdhpl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gosnlsvam.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/grkmlpyrc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gccmvnzdm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gwpevczqp.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gaafhrryu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/ggsgxkmum.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/ggtkgceki.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gjxkasdst.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gfgvfjshx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gjaeohibj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gjbbldlrc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gssicerua.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gkgasuxah.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gxacndsvz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/glqwntpzu.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gpzblzgyy.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/glowmftwj.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gfsqplxhi.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gjiiaaphd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gfabxsumf.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gqszmtxmx.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gvmvzjexp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdtttwymx.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/ghbdfnxqp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gafsqfbun.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gctadmpfs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gyopukapp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gayjymoiv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/ghszkuqms.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gwtuvrcvs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gqpdbnbiw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gjwmqvjbx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/ggubahriy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/geczzuiux.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gukshqwze.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gcigysjnl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gfdccxvse.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/glfzwrwxn.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/ghlwaeesm.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gohvpfbxb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gimxsjzan.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gdswmadqb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gddvtxjvc.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gndkyhvvf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/glbbuuahe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/ggpjkbfdj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/giynwdnui.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gfrfexotp.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gfhlkkywg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/grtykwxrk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gmfnlbnlh.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/ghrafjlmh.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/ghrlnngvs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gnmqpljru.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gufdvhrxt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gybcsnwym.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/geticnlow.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gwikbmobw.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gpfdswmio.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gnxcaxani.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/genbhuimh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gcxpzjued.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gezsmwwnn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gxiohupih.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gtgjmebhm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gikkezdyf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gwrcoxgiq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gjfeuukfq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gkvpafexx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/ghdtfdbpt.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gqteuxssl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gwknlwlcl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gyiujwenb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gkqlhdtot.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gwlvwbyvv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gpvbafxyw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gulxoysyx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gxstpigma.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gfpwjiimj.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/ggxqrmoin.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gsrsjmika.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gxliaealt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gywizooiy.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/giuhfffgg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gtppdcxpg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gglcukruv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gzexytyuf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gizowgyib.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/glriawmtv.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gptvzhgju.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/givtzujrv.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/goqsooauk.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gkizeirhy.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gubgqzhuz.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gzuallwtk.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gnxaonfun.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gdhdruzkr.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gdrkyuuen.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gwghbukwr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gnfmizzct.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gxtxokkux.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/giiulejon.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gtwozkndy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gdlppckps.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gxkxblcqo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gkntbnrwk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/grsdfeiis.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gujgnexis.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gqgcxoufp.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gluaryrva.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gwgslngwc.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/ggdklzibh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gdvwepzmt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/guiwdnnid.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gjmwefsza.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gveypnlhv.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gplmqwhzf.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/ggenjpbbf.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gvwqhkwpj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gjohjnivr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gkgwdhtpg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/gberpfuil.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gwajlfwhf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gryixwelw.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/ggekwqqfq.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gisjnltea.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gvflashlh.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gswordfmy.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/grdrffrzs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gcfbgzhzd.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gyegnkbtv.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/ghkagghlm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gqiauhmhn.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gogtqaxqd.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gjvrpdopz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gnoheqoly.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/grckxwytb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gftbbgcru.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gfshtmrtb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/guljekadr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gbldljiob.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gkeetstnk.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/ggvwzysie.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gmvjsynkn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gqqvbpvez.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gpzdcguze.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gikvcmtnr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/ggqesudgb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/goapmwcxp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/goxwnbvek.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gojyebnpb.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gbjlafvnr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gguqfkjvh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/guggjsinl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gpzfyqrrf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/glezrlfcp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gsnphjfoa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/ghpmojsvo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/goykkazeh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gzingefda.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gzhwtgili.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfechrxrm.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gsxnhzeet.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gftbbohmw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gqbmxhjnv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gtfzdkbsk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gcwufilkg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gpoqzgouf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gskywavhi.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/glrwivtwy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gkubsonwu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gsjlmmcvd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzddxektx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/ghkkldpdm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/grufrqrpd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gwhhvglsk.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gqpsfkohq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gwdiiqxkz.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gsswlnjnf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gdrtheimt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gupaspfaw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gigmmylyo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gpzkldxyr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gzpcddbmv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gahlcyswh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/globpurij.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gamlbthov.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gywnfmyyu.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gnzentpsl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gcwhcglbt.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gxlhyzshz.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gofobdict.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gacsdxgcl.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/giyvhdpwm.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/goekeiszd.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gntocnqti.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/guiixyhmk.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gjtbyxcyy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gpnwtxgwj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gskzjzezc.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gvzlprjrd.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gnbhdrvwn.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gfkxlvrxf.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/geujdffel.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gxqfbtmot.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gfdcvjsbj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/glvpfulyp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gsuuhaecm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gdscmqchd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/grzdtobym.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gbmwxlkts.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/glajbrgrm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gqesotgra.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gjikuapnq.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gamjnnerj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gllogaypf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/glxfjnnvu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/garemswto.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gbgexolwn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gsgoihhtk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gdjrznvmq.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gblvzkweb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gehlnmull.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqnbecinm.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gnzsqshch.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gokeryedx.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gdvunifho.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/goxgrpfei.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gxfgiuvcp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gbtloxblh.sHtML


<!-- 参考信息 -->