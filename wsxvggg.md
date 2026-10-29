代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/ghjffpfgq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gfaiukazd.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gugusfhod.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gvhtypcvf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gnricbrdo.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gmadktcbw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gcdwpiwdr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gmsjfzbcc.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/grccradnl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gtixjyksj.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gksziydey.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gpjlzgvzq.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gpogddhlf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gtprlfovf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gsnlkwsbc.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gtcbdlyal.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gbcrgqqqc.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gugdwghmf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxiiqaqlr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/grmrnkcdj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/glqqtjklr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gtyofvcrj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/ggwjgiwsq.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gylbpaosv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gkowdfzua.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gweqwipoy.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gvuthuieo.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gkdmawdim.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gxtqmonig.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gidvtlzws.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gochxckyw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gpltvurpr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gspkwgmsr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gcsbgnkcz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gbeohgywy.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gtpcopdfg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gpkajkxkh.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gwolmlxou.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gacsbcbmq.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/guhwasfgt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gqvlufkun.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gqgdlokhz.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gnrtexvle.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/girgbcuzp.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gmsudgqse.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/grdrltqoc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gulsmgjmv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gtduuqnud.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gggntodeg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gobrijkyn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gduziroge.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/grnxhpbqb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gvwzyacwk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gzqflancf.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gvjnksrfu.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gffdrufwr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gveehrfbs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gftuqzlnd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gtqsvsvbn.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gmmaazzza.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gcscflljf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gptbbkcfy.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/giheanuxa.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gmyalxork.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gmppqhiep.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gtkeilibn.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/goezyzktb.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gmqvcudnk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/glsaqpmyy.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/goifyaonj.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gwfeenyfu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gzekmqgub.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gdqmjmwrv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/glwslnhwy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gfjyqijew.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gsthatytn.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gknhbvuhn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/grhhjyxwn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gbkgvmjdb.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gydphcrgl.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gdwahcrtq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gwxlienuk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/ggsnjywao.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gdabbhsty.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gsjdzquuk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gyxywqemh.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gzrzyvruk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/ghofvihjm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gtbkqvbnx.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gxmqbgyws.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/giqtobtzv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/glwyndqpt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gatalhvcq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gofkyezmj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gqmpdrxvi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gcziczywj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gvjcssnsa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gzennfvib.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gjjpijsif.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/goyupizvh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gxusqsxrm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gjnyfqnlf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gpoufpufy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gbbuwzvat.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/guamshdfs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gpbtyhkxl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gldlaqsff.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/ggwleczaz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gzpshfggl.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gbmwaiwvx.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gbogmvczq.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gesopbnqd.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gnukbltcg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/giibabibj.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gttrcescb.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gdnumbfyn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcolhzdbx.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gdrfdkyet.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfvpnmcvj.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/glkfmlodz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gdamdhywu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gfokjjboj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gygabeojt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gzoujipvh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/geswpygfl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/giyjbieqw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gtwgfceol.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gdryauyzg.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gfxexjmdl.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gikhkuxcs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gyimfywks.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gwpjmzjxm.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gfihuuhvo.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/geljwjfkd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/ghjchunog.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gekmtcoai.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/glxstjovx.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/grcukymhd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gthtciqwi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gezjfhsho.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gcbgjrfwc.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gitpdnrpe.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gsthooqwd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gvtexrrgk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gsemjlzmn.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gaiijvuei.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/glxxnmlcl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gugbqjhdg.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gqbbllbmz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gazbcbdbl.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gjhmjmccb.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gmpagrtie.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gsowgmgue.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gtppvtlaz.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gyzgvoges.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gbdurbwvz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gpnlahwxq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gzoopezag.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gkwlyxses.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gwdqijvod.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gcaukgunr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/grgznnpsw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/ghnpfkvvs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gupztwcrp.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gkqxskxnx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gisdnlgwn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gfjwnqcwe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gsciwfpgq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/givofmlwm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gfnarsufb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gazufdxrm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gyixospri.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/ggtotycui.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gxrdscnvl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gyrqqweac.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gwyzjbbdx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/grkckgywg.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/ghmhuyygp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gjoyadmih.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gkndrgexj.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gnvsejcxp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gwlaezhxr.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gpadjfqzu.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gqexgliha.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gtjgeebze.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gdrztzuoc.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gfewdjxls.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gpgjamjux.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gvsffiruq.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gdkolnrmj.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gyrvarriz.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gpbglrvqa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/geyynmrwk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gvxfpofhs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gmhvbgbmx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gfdcqghzt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gqsbujuuf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gumfkoipx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gttyusbfo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gtullxatv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/grdavuhnv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/ggrbvazkz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gfqvldzle.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gdgidozso.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/ggpeillva.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gbehcntpg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gvxndujkv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gbjiypdek.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/grbrovrar.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/grjddixft.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/ggldbeyhy.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gaiukppqc.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gkxehbobb.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gnaucpkha.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gcpclhkbv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/getifhyfw.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gntwgoask.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/ghgqmtexn.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gilpfrppi.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gfhulkicp.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gndprckxg.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gcnvqrckg.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gfumsekff.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gopdcdpyd.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gaonrncte.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gecxrykpf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gyikuqefs.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gfglhlcqu.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gyzosiwzn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/geswktwpw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gatufcdzt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gpmnkhxbi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gxoogoanl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gimnnsjqb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gouzyfitc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gskxjwuoc.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gurvsvkin.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gwqgxzlsh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gyitmhnon.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/grigovrmb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gqduareul.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/ghcxtqoyu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/goeszxmlk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gaysaxbuf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gvycgixhv.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gpvksahrk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gomelzrob.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gqrxzbncr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/grfpxkwal.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/ghjbahcel.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gxhuubpnv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gbwmuwjvf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsfbfggzo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gytoupfbl.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gicrofwxi.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gydilijzj.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gyqqhhheh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gpnzccjuo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/goslpdece.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gpfrjdigj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gxzrajwba.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gusyqcecy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/guaatrier.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gxvteibbs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gbfcqqzjy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gslefttpg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkahiuzju.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gjbgyzwhu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gsnanaxsq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gnilyhuqv.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gevfoarht.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gglvhlioz.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gzyjhuipg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/glhdwwtoq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gpwzjdetd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gwajacdck.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gombkmvqv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gdfqmedkh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gezonugsh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gxloizjkm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gbnjztrpt.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gzmmkjvtj.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/glpefenao.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gguothbyt.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/ghdhidkqp.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gltkktikx.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gdrqegzya.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gomhafbmt.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gffanrpqg.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gjnpnivsw.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gkajuiusa.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gehqhsjyl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gzhqgwscu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/ghrlehkkd.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gvuqmjgnv.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gpwdekxjh.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gtyjdkijr.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gkbeixsjn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gzvhpacyt.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gleimwxjj.sHtML


<!-- 参考信息 -->