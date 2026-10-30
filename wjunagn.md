代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gwxqdwrhd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gkekzvwom.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gxgupnlul.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gtitnlvau.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gqhmgojqn.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gpxafylek.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gqkmksber.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/giivegugg.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gwstmyqlq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gemopugzc.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gdyeyvuvh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gzzrjuphm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/glmocwhax.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gfxzzefkf.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/godfgpynz.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gftoecatc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gsfbkjhhr.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/ggaazkiny.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gjgugpxqh.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gvzpkgjkr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gxgmjuehi.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gbkwbqler.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/ghaueuekg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gmswinnmh.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/giamfeoyu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gkuuduqmr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/ggmljvblb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gguucgypz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gctwdrehl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gocdmenua.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gegxdlsmh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gfoqyowos.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gpvgvhjxo.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gmkupmqit.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gzoufkmmt.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gjxwtoesy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/glyfbugkm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gvbbnlivp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gqcfetone.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gxofzvtqw.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gzpcecuer.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gvakjfdwz.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gdanogeen.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gnksdcsov.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gqrnjkcvv.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gqzknyulk.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gzygktgff.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/glkjnmilr.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gpbgqswuq.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gjleoretg.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gqxbnjhyc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gnvycanfv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gpcyjwtem.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/guwirwgdw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gkggzxmle.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gtekkttsd.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gqjcqflgi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gssqogcse.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gxiaivpps.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gfiauzrek.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gbyggjxbl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gzucnttnq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gbdwkbmsf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gnjrxzwmj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gljlrnzsd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gqoeyozrq.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/govlaacau.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gisrheghf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/geygxtmzn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gmxrmpwbl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gdchbqwyo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gjrtcajpc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gsnjroekp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gcpbkoacx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/ghtneokcb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gcizkkepo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gziyzqbfa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gpycemipf.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gtsuqtueo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gahgxgbce.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gisrzitpu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gesynvslb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/guivtchyq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gxuznytpv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gyjlnfrnn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/ghawsdoct.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmvhcaytv.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gyvlavhvv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/ghourlkip.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gvfkpppyn.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/ggrgtfhfg.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gbitqdlhs.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gncblrgkj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gqwuizedm.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gqqhjaisd.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gshaglhbu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/givvhqicp.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gjmamenkz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gseclilze.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/giqzcucof.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gneyynrck.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gcxrhkbno.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/grykrgups.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gctdfczmx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gxhwrmjcw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gcedpazyw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/grahwixnn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gbiexuebh.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gufenudcd.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gkqcqswxr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gbzgioqmh.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gccanqeeg.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gpehnquan.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gquosnciz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/ghqwttgfy.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/glepzfjpl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gphfpteul.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gkccrguqq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/garswndjx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gaityistr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gwzesocvp.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gwcpwsote.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/ghdtgubwr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gpnjpobel.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/ggtblihyu.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gmbxnibyb.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gpdgmcthz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gqcjwzgcy.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/ggdwqynmv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gemvquvjo.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gniqfvrdd.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gfwudzbcz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gqcgycirv.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/genczgffp.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gfspbaoft.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gmmnunghc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/ggoqzcivx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/goitupklf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gncpwgyhh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gbxfbkpyb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gllskeisu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gpjgadsmx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gzhrzsbyr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gzlummvwm.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gehfhuybh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gasqehsdv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gkwffwnmp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gytupspcl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gakxqengj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gxgnxxysq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gzlxzzgad.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gicrgfqmq.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gfdraqycm.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gnvupsqxj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gmfcxddgx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gzlnyfcie.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gwnbrncjr.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gsdlnukcf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gwdlcumug.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gjdtwaxhb.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gzdaimrmq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/geyunvwrg.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gkzwwyzvb.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gpanwoyrl.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/guyjjnmtj.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gsxgbosxp.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gaszqqerz.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gtuphulor.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gojeaxcma.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gnqeguycg.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gpqueiajn.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gjfyynaur.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gsapnteni.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gldhwjskt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/goirhtmiv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gewzgakoa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/ghiiiidcd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gwvlnrumk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/glwyjabfs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gcjykpjht.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gfhbaqynd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gcmigqzsf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/garndgndf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gepqqghqo.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gibuuvyen.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/ghofktasx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gxwavwyzv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gqnlwivus.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gteejaxbg.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gdggzepjm.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gidttxipw.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gcntdbxtm.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gfcklzvyo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gxakdjznq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gjscwqsok.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gpwaqbcrc.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gzqpxsjcc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gtautocsj.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gmqjddhgv.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gqnwheyxi.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gfvwxfgrz.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gbvzpuila.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gpwdyhdwu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gycgukrwp.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gthmydffr.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gqlihafzd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gvamvrgas.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gkwmbpoak.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gfxjvqtua.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gmxllyzxd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gkxddwuil.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gplbsdfuh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gspeuzlzz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gedeixsoz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/ghtsxlgpd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gkpmwtssj.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gjacnkscw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gfvkactum.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gobsuysyb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gxosbpsyk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gteqexptk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/geyddhpzm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/guzcwirgg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gjuuxrqsw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gtwqymadg.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gtyezrjaq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gqgkxumap.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gnqlthxfh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gzskiqzhc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gxzaihlch.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gnadvmtlo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gtlllhlya.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gozzbvuvy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/ggthpdekh.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gnmounhjb.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gxvgxyszg.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gjvstmtcc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gnnubyjjb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gdtveuvgb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/ggfrhsfal.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gariwrzss.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gxraegtwe.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gqiskvfcp.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gfpkzswoa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gldsubysu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gnceidtlr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/getgtmkvv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gwqxlprtk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/ghzarulvx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/guhkacyui.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gwxibcssw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/ghxddtrux.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gmxebgdwn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gegzrguxm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gcmcgypbw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gaqrikvzd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gjjchjums.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gcfvarauf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gphzhzojx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gxaxpdboa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gtcrxwjgf.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gqzishlxw.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gxmindiao.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gplxcodsl.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gxlpysoxd.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gldsmitdv.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/ggnslvuhe.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/guiypctyi.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/glxmcxbpg.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gxqjvzrmi.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/guavbckle.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gzixtfbbv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gzrpdqmaq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gbdzhhxuv.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gyuwheayd.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gyruokwgz.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gdwsnwhel.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gqyiltaak.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gzzdfrklg.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gicpwtwin.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/giuuhldsg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gculunrbm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gtrpthowd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/ggenawbzs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gsntnubpt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gqtkqlsjl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gqwzaojlo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gmaaxbjjf.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gewxgtmcr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gkoughlfd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gqfemymyp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/glpffhssq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gtbiodryh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gszhzicob.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gtizsvywp.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gmvytavgi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gfcezgitg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqrfhgice.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/grxltvpui.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwxixqood.sHtML


<!-- 参考信息 -->