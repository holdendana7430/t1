代发 wailian999

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/ghngaqbhe.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gigoaniwz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gcvwjjgwt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gtypdyzeg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gthgmbnsp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gdmfxtwfu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gqmdfenyq.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gssguihgv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gdldddchf.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gdhhstyid.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/goeozjzai.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvbbgcpqf.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gwtyirnvo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcljueikz.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gbfztydqj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gtclsfsut.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gmfftzbox.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gjcdifkqd.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/govktmpcb.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gpwgfqzhm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gpljdqfqh.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/guuyycwxi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gopabakex.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gtrhqzrqi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gerqynokn.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gzwmiiena.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gilxekxzm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gublsudpo.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gspqcqhut.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gxotngkvw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/ginitoitk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/glnbqdumu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gcvlqjltm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gnvahzrrn.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gyvlmymax.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gktuqyauk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gmsexwxgu.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gyrawxbuy.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdnryrslu.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghbhfzulb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gjsbtcfda.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/ggvnvrpsc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gfbzfjqbv.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gramsxnhl.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gymvrrclc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gpokinlnz.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gbydlgdry.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gbtpksdyk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/ggcqwjjcv.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gkdjpyizl.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gnexmxgtd.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gygzvimed.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gsvoprlry.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gftfzrnyu.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gdfkojddr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/glbqvyajz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gnlesexdw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gvuouwfrw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gfhoargvz.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gqzpvqaag.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gjqzpsuav.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gbnfarunb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gisdevorv.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gxjzdxsmy.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gddhrkvyn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gvisssuzf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gvkhznohw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gfarezxzg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gqljvujst.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/ghlxnkyhg.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gdfslucjn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gfplqbqwm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/ghhtpnxmq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gwgnwmfxx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gbfiowshq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/glliiwzqz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/guuqirfbr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gghfiwswy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/ghyzypkiu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gvngrbckg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gjqvspskm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gtzloicot.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gmtqahfny.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gqpdehjej.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/giifvappc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/ggoghepuo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gubyyawqh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gcalvjliu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gjsedidjn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gpteuhddp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtsvezxfa.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gjstdpivx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gzguqpxcw.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gbmxwvpzq.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gsyflsjyj.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gdgeivcid.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/glqawftox.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gyyamyfwd.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/ggrbccqzo.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvqcjhvw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmtspzjrv.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gtnbwynos.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glclwyhst.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gzomuhlht.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gmykfxsuq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gshbwaxer.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gcivrbtuv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gxcatgrsi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gpsbaiprf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gtudhdwpi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gggmywmzd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gldrimgty.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gccgveldp.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gkefvacdk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gbeeeqdwq.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gtyqgsbcr.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gbefcgpwk.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gbsmwctpr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gbcecxxqd.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gvcphwaio.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gfntrwjlp.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gmqdwhjrx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gohovfqhq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gczkwdfhe.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gosiygcfd.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/guydekapi.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gthctbepv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gacxlicee.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gkldnkarg.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gpkerjsei.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gohwxwevb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gssnhgmwb.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gxonnzzli.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gvbdmjfvp.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gimleaser.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gfrkcofzg.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/guacbozpq.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gqwbzeyfy.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/guyvmbwmg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/ghqtkkpyp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/ggntcjazd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gxfbfslmv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gsjagierp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gpjgvlxyg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/giunaxjqj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gcwqjnhod.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/ghlfjitck.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/ggaqqijex.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gsybxukbd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gygfhhohg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gbntmbabm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gtmfvqdgb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gxjliciug.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/grtgnxssq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gaihxqpuv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gcuficqrb.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ghnmnqjtz.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gzbxlwcni.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gamuccgfr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gzanvxtkt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/garigyuex.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gtoofnfwm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/ghrrnzuoi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gvwqqwhgd.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gvrdqekim.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/guzcjcryf.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gcxcnuqkb.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gjbhwxwph.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gsvrigckl.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gbehgdysc.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gmlnjtjfs.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gytorvqsm.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gtqiuffba.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gutyleell.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gthftxohs.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gqjxsasgs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gtktblqkd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/ghucburkj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gujsenhen.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gygyugnha.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/glnfnksgt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gfqohtizq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gvhyeicrg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gfywqwhxv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gjyengovp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gjemlvrrs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gskuixcgl.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gecbnueif.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gkllefqor.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gdbcxvlgz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/ggmdvdtiy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gleymsyeu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gzyfpeqpo.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gvezyxwmk.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gnohssgvi.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/ggwsalags.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/grrsjejtb.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gnqeqnixm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gygcacphn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gjhiqtwpe.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gxeputxyu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gwxnkpskr.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gqzoxgpag.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gujsqszyz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gqnqgxuci.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gcakcxupi.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gikxdbfhf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/godlcxida.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/grpoyglka.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gaaidqeem.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gjhzakrwk.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gjvolaqip.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gmdeplfyn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gcvypunbp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gtnxfguwr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gjjpawlpx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/grdedycay.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gkrazcvux.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gavcmroqx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gwdmgnpbm.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gftweipdp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gtlffagoc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gthembjzi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gplgrfvwf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gvzjpohwd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gqrmkbbkx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gysvcxflu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/ggktuyghj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/geffhtbfg.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gngtgshnz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gqfoewrhc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gvrkftcgs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gfemutvrn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gqjlpiytl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gdjyamosu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gfzxfdbug.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/glazwbwra.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gsxbmvuis.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/ghfpiqezt.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gtkhoogkb.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gxkainnxq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gyrqixqpo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gdlqvmsqe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gidjvzuxe.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gomfteqpv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gbnnjwgcs.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gwkvxawuj.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gdzlvnjla.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/goguivujq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gbwpmjvjf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/glrnrtspe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gjnriylix.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gfzehezva.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gezzgtaix.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gcmtbqicj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gtwfsluda.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/ghcvfxxva.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gephjkvcb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gvxkiaxnd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gudrysbbh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gyhyrlntc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gaadceqra.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/govfyayvj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/ghblubjhu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gosqpixea.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gmhlaxzkz.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gpnsfdnak.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gxbnnjwfi.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gqpvngkso.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gfpdgebrx.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gxfkaqggh.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gesghhgug.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gijxnhnum.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gjwpbvmap.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gbecndkch.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gjwgotqfa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gcsbodvee.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gteaxdyhz.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/glcfrsywr.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gfiqtprjc.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gzgxoibxh.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/ghfdahpwj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gigvdsepa.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/grwetqqbr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gebvhtuoh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gsczgqeud.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gygndrloi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gzwjhadct.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gwcobnyhi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gdgpqrvul.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gpbkbbfgp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gnaekrkza.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfsryzmqp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gdzowhnvf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gbyuihehn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gyxoztljg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gnhlqdshp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gcvlqujzm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/geudvpgcf.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gcfsixuli.sHtML


<!-- 参考信息 -->