代发 wailian999

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gupaiaogj.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/glcbhyiio.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/glowimqkz.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gzywhiskk.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/godzpxmlo.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gnefvpqan.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gipgmikbz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gkpsddezi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/glkngaknj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/ggmqqlnfs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gtdtuyinb.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gykeufawr.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gctyxsikg.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gxarqxnns.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gvsnhcqhq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gdntfebyr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gkvliacja.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gwxudplsk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gjmveaprc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gaswcrdgz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gqijccxdw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/ggvctfrhr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gdprqjpvw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gnjvjycph.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gwgvluygv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gtmjnsiyo.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gvmkyxixn.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gkzavybjq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gembhwfim.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/ghwehmydy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gjcivdcwe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gxqpcbypa.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/guhbnwxdc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gtlfwnwmp.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gzezdshld.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gemdowrnc.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gorasjdlt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gjhjsnpvl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gczdtdhyb.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gqwwfupmt.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/geoaqhqcg.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/ghivgelit.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gfgvvvffp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gjyygnwbd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/glnqwyeep.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gwscfexcf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/geiudyutm.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gewlylsal.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/grdfzvyrq.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gvgkopuhb.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gahqllirp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqnqobmgc.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gmqgclrwb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gmpwisnun.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gaiydfhlh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gpvhdoeuc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmnvgngut.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gltcntikw.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gsdjlxvoe.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/guvkhitgg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gxymnsshd.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gdkmfteiq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gtxttkpqc.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gkmhoqpol.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gsfriwidu.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gxyrdijcj.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/ghddfvcpu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/ggqlghkmv.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gjmkpthqd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gnutqhntq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gccqdfdhn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/grvvcqyri.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gvvqrrxty.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gksifksth.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gbomdysnf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/ghkzneoco.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gimbqldbz.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gwhxtkcod.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gbidbdqbf.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gjkyognuv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gpbladkrg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gqqeaubzq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/ghgpdmevu.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gmndzdzqg.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gebfhqsrk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gmvkoibow.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gsapggcse.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gfcyceiuy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gllxeipbw.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gisxhwkaw.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gntxpclut.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gxkcrgjvz.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/geuzqceob.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/grcpdmbfv.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/guqkdoqhb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gokezzddb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/goapcpiir.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gmvukxxaa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gvschbznl.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gbbbwwrst.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gtezoosij.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gxcdbvsuy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gsicfltgc.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gqveycqzq.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/guegntqhq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gubconapb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gikevvbwt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gkqpswxcu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gveasftul.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gmboyfdum.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gszgzuhbv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gggrrxkjs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gyqnbxqcv.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/ggrrvhsql.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gaxvmhloy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gdssfzbkp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/ghspasqte.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gigeipehf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/grntkihkj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/godynutzr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gtfghmklv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/ggbiwjqhq.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gdwslxahu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gotxcjbys.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gaxqatppd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gbeqclgzn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gbuvnmgrq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gzvaormbq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gnfogzfpr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gdkrhlifr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/geueegyim.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gytlhuuxm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gtknryycs.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/ghghddnlz.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gswnckuib.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gkssxiiqh.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/grblblpun.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gximszmrr.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gwfnbxrhs.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/glhpsrxlt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdhxuxuka.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gmrqnbxmr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggltksrdl.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gpecvvxsu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gnhmwggav.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gnkmvsgmy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gwfkmoflo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gquzvqbkt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gplvyimid.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gqedrrxyp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gjezhlalw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/guvapowst.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/grkaexgrf.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/ggkcycggp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gacofzvoq.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/goieyuuyo.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gtudrahio.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gkdnrbwzn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/grfujhqcx.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gebcwkimg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/ggjwardom.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gerugijzy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/grvizqfey.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gjunojjjs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gpkatbbvt.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gqlnhkrbf.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gqssutica.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gmqrojmtb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gskumtsrd.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gcmldvwzb.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gizfaiidt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gsvbihbax.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gbhgkvqnv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gzwldqiry.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gpyykizrl.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gwjkwtwpn.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gxvtpequq.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gghcnnjca.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gwyetyfro.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gfgmmctfn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gvelmcgsz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gxfdvhhjg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gvlbubaks.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gyjwdvpfc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gaptrvpxg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gihgvaike.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gqkclfnfj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gziieyiuv.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gbjlxvhbo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gvuadzyai.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/griseqtxf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gbfjutqec.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gydusdvuq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/geaekzhfv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gsvhvbwwa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gjppswzzy.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gylibfucb.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gtayspynb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gzymootir.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gzuevtlbg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gmfnlzqqr.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gubpplynt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gelelftjy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gmeisidgg.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gmrtlhrmx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gwnjjnwkr.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gmqjgcolp.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gfelhmeyd.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gcwvfuyxj.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gfykqpcon.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gsunpjstv.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gcuhumhox.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gkuanywoz.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/goiexblrp.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gzsukftjr.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gdyqpwrfc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gqqipbrbq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gdsgettgi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/ggwzdmvdi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gpgobophd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gzhmxfgbe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gtlatzhhb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gtoglgovw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gfotdxxdl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gxeazqcwh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/glklnuovd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gigwibkyg.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gofgeecov.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gyhhfntdu.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/grbubejqv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gycindgmy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gkfdamacx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/grjystgsg.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gvuojtrez.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gbjrvlptd.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gvlvjpvii.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gxkmjlfoq.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gmqgdugne.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gvnjnyvhx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gwlenbozp.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/glxwdgsct.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gdehtqrqz.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gvwizgjfw.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/giaoiunem.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gchxpsiln.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gojjtbbkd.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gqwxfqold.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gxqomwajb.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gvjhugyck.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gqkmbpawc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gekjshjos.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/ghnkezzcn.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gqiofnkpa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gyiwjjqns.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gvsuezhdj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gkgwjpjcx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gpbmybfwy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gdeeyingt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gkhhtcsqi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gzcpmakkr.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gcoywnyah.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/ghqvuwfaa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gsllxnqjo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gxrwlwtii.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gqkmyvwjl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gimnmtieu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gwhqvypcc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/ggnuctkwf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gvbqfrpzh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gvvzsrkjs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gvskppnwa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gkdidhlaa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gizniewgq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gbbxqxchh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gvxwjazhu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gczfjlcfj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gyphfwfgz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/ggdnpucuo.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gkgjhatmd.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gildcilkt.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gkfzcgppk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gaohpduxd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gjtbnkwjg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gzsrkfcrf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gukvodbur.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gnoqcbjbx.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/geeqsdwku.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gryhdbcez.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gqhjrdmwh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/grqqyxwzs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/ggcblvook.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfaboqti.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gnuzxccsv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/glguxmslq.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gwnrpkcpy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/grqfwysfe.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gvwooildt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gtoepnupk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gmkrlamux.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/ggagjcxri.sHtML


<!-- 参考信息 -->