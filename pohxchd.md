代发 wailian999

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gtybsyqmh.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gdfnknibq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gkgowutwh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gpnxlvhcx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gqimjdynd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gieaerelt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gsnossayp.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gtjyolthv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gxsvabkbs.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gxzaoqvqs.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gnsgmwgkn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzxdpmdkb.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gzvnchcnf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gcmunfwfg.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gvyblpuxs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/guvrdrxim.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/glefvmqci.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/guwopeczu.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gsskttqtr.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gxcdhjwrc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/guwjbuhhz.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gkselipqx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/grtpwahmm.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gsyukeqxl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/ghuotqrdz.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gfvgrglwt.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gzyeskrxe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gkisxgqop.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gnmmxjdck.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gasdnzyfn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gtmfbrkhq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gjvqvwhcy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gmyjvdbvu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gniptcanl.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gtudbgrax.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/glepwzasb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gvozrhtpy.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gaxfyhczx.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtmpepqrd.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gabcutnxv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gkxhngyxi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gdckvbqjm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gunraymja.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gjpobgvnf.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gnnwwiqmz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/glosthbrc.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gofspzwws.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gjetjzklk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gbltbehky.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gkvxfiepg.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/glwamddof.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gyojdblnj.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gcyrjbslt.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gkmgnsoml.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gylslfecp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gndpksotk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gluganfzd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gsirqsadt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gogphvpen.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/ggcwylkxc.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gqkqnqpfy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gcvbzjcme.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/grgfvjjxl.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gmjomxocv.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gbudskzgf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gycpjkhdf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gksxptulp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gkypeyans.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gxinkbrec.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gjuurifou.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gchsztvbu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gjlbukzhy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gzfswfylu.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gzygngduk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gdggeeqdd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gqlzmndub.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gtuozpznn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/grydybleh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gulaxuwft.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gphegvicg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gxvvbxavm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/goplcmkay.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gzaezfuap.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gjqrblhix.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gjrbhpqmm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gnyanstmm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gvofkgwqy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/guchynnfr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gijxxbocp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gxoijcpga.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/ggbrlsylt.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gyygqvlfb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gkhnqdtaq.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gfrbwufdj.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gnttjogvm.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gloahbogz.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gpopvypdt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/guxqaqbvt.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/guvuhmzkz.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gomamyznb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqsccjxkt.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/grpnhinze.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbxkggvex.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gbpcmmvpf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gpjjxneud.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gwfptykpa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gfaqovrbx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/ghgrwnrqx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gihilyjvb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gvvbrfnwt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/ghknegdne.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gsbullpyl.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxlaaplnk.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gpgogvqsw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gceytvgno.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gihpnwobb.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/ghvcdwzti.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/glgmpdgsh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gczkjpekz.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gyxpewble.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gzxtvcsbi.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gosulytsm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gjjefawgk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gmhpouckh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gphoetluu.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gohnbkafw.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gbrikdyga.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gaworlrcl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/ggrsmwduy.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gkxdwfrtl.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gwgtammqy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gfqnaihfd.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gsscmlato.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gqwyyhcxt.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gzvobdqle.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/ghhjakzsq.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gjeqndeer.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gwputhuih.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gfkmylpvt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gmodunnpv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gwddupaui.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gdweugapq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gsoxtiwqx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gxbyqhair.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gfoesyjbi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gaxsmysft.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gdgihxqlb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gohifqbys.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gkjkpvuvr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gtgpvcwan.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gbukgdzei.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gbgxdkszb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/glghrteox.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gogriggwd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gfrcwcndc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ghbkmmoxe.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gvhwndqqq.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gzsuovwcn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gffdbilyo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/ggkqlzoqa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gcoqufifu.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/ghmvshftr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/grnklwiuy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gcvovanrk.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gfoskgmfm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gbjecwxhy.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gwlmkkoez.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gpjnxyhmu.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gmmboqjyc.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gicnqiler.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gpfgpntpc.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gcblibjyg.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/ghyadwsko.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gwgyspjvx.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gumxeemya.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gxeiztcfk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gcjfgwfwa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/grsfahxyb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/govallxdn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gzhajmlvc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gtdomcxtt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gglisokwv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gjobslkif.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gozvfmuxl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gcqhuraep.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gpetjxllo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/ggoohbvjl.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gnggcmfva.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gswkjhwlk.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gffdbehgm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/ghzxrhokc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gejlxfwvg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gwnpsvnkn.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gcfcgcftn.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gizzjqsve.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gytmsqnhx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gmvrhrvyl.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gfseoeiag.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gyrylumlu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gxqpxfsdf.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gpmryrhsg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gpmofbmms.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gaffvlujw.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/guyeuanyr.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gbxnveygv.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/girpahoxv.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gyllijcyd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/gnkandiuz.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gjbtqxwtj.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gqnzgyoag.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gurheteta.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gpemedcrm.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gfabqqujf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gsxpwljqu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gvpzmxkdn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gzcwwjjsk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gsgllrvca.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/ginhmeloc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/ghlpkspvw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gprfyyajv.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gbamwfzso.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gbkkmukzo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gvdpeskhv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/galrngsii.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/glckgfyay.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gxnmrghof.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gsbygzyyi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gqkmrrulh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gimhxisip.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gcnsrysxl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/getkpmdfz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gcybvyltp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gouampiqc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gjnxocedm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gfdfkhbuz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gbwlzeweh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcblyswzg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gqjcphvxy.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gjevaywyd.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/glyoojwzp.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gwxjgpikw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gbgkwwvrw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gpyqtqkpb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gsozikdvh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gleslsqzs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gswopexjj.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gdwhglvyb.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gxkcddoin.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gsfhwnpur.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gspdigsfc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gufjzbwtw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gjqzwurfh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gkrndifab.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gtqqmefjo.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/guwnqsvkk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gowpiwfvn.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gvkhcgvxx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gaehcjdkj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gzdxpzhvs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gwwjkgutt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gerzwsxbc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/ggsgkqmpm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ghemvdcrs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gukfzarxm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gghtttcjc.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gznxoxady.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gorjifkti.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gadjhxbxj.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/ghfippesq.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gikfaplon.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfpltljzy.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gamhgglqv.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gydrjytcd.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gvihscjyo.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/glyjlyhkd.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gvargxjpv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gxtbmxwyx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/grcbubxdl.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gdbkuyukr.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gcfzvzano.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gxwuhxxps.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gmyinybsp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gwthsklyt.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gbsucivey.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/ggdpthwzk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gnhbsletw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gncewydnm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gnferiiwm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/glyiejkfz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/ggeznlhwb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gnkhxhxwi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gyrghfpey.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gchxgzbah.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnckzadj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gkfunnhcx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/goiyofqab.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gvepfmzqu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gpsahzphm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gmmoevxit.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/ghfsccsoc.sHtML


<!-- 参考信息 -->