代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gquriygrv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/givrnokuz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gdxzoaoyt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gsjgtbolf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gtgdqxqmh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gzkhozdlq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gwodyrxuu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gnudwkvkz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gvyxqvhqr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjaxwengb.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gklrodxax.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gsyknlwio.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gjsckdtqp.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gsjjkkarg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gpvxcnceq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gmdinesif.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/ggmrekhfj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/goiteapbr.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gtysaulre.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gixnibhyt.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gepdihyrs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/goezuwscz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/grtlbnxve.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/ggxukvzaa.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gwoscchfc.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gtohpnsji.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gxmfnivln.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gbaflqapn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gqdnohqmj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gpazwkpsi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gkdzshxvz.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gzrpesmaw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gbylzfxws.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gnnltftiu.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/glusiffak.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvgqoyggf.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gguuulyhm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gxejrdsej.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/grkwszass.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gqkihmrra.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/ggmpbscsl.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/govdmxgqo.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gxjghtnxj.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gaqfumous.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gdrxulzxp.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gggfiytwl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gigrqbiwm.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/goqsrrumw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gvnppypgg.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gwuzszvzz.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gciwprjpp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gjjshydqg.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/ggwkfggxu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gfdgpaaxp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gmrggyqjb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/grdbqbojk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/ghkutjkji.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gnidmflwf.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gqtpgbewm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/grigqmsvg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gjehtsvsk.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gwkwwvbxa.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gqxoummvv.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gjptopqbd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gbrmuadgy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gpstgzvsu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gadhjeqrn.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gcdpzuxuf.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gqplbaxio.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gkcckarwj.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/grxfqrnxn.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gusuybygt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gscmshekn.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/guzkdqjzm.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gotdloyak.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gqitkdkqh.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gachjvwha.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gbyxbsbxd.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gqcidmuwc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gdjzgczjf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmwnxnpzl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/ghuuhhipz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtmhaovxk.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gwfrkzior.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gqyitlmrm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gvxolqnvt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gxdznsnnl.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gotqqakus.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gqogcqmco.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gfczqxphs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/glkmiteld.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gnmnbutex.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/guswceecl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gfuszizzt.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gfkcjlrwo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/grudkpskr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gtnwlidpi.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/ghucmmepx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gnhnglcjv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gpycxjeou.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gvujzfcjk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gepchbxkk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gcdxasyti.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/geekmgyig.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gcaxnptom.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gknuupefj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gtnyzdvte.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/grnzarbhu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gqykylkhp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gkitgkwin.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gzjcbczzl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gbfqwkhrk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gwwtsmziq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/ggswgqbxj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gdbakezmo.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/glpbqcdka.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/goqbloygz.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gntpsjrdl.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/ghgsoxxui.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gozihzczu.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gfobxhqgc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gaebkzcor.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gixmhfbdo.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gnzeesmty.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guecsaoqm.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gfvibfscg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnvzxlcif.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gixfkksyy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gzykupddk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/grdlxezqs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gulxuhwtn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gpowxjmbb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gzojckgjo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gvwejbfcs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gyxkvphjp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/grxqtpdzx.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gqdzqyfpn.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gguwztwio.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gcmorfxhn.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gsmirzxvm.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gifaxslln.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/glacjxgkl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gudzghlwq.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gomukmvdc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/ghozbgwkp.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gasuufjvk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gsyuwtylh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gbbsozbyg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/ggcvqwhqh.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/goiabvlke.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gyxumabsx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gekyevigm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/ghdrytlst.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gmosbwpoc.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gzqmpbzcc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gmiiuogjp.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gglqaiaer.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gwgctghhv.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gsofvhnck.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gsbbnwfiw.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gxngxjyfd.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gjvcnoyey.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gnihygcub.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gticdqzsb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/grospodlj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gptdtneco.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/grmwadjge.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gpexbfund.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gohdkiarh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gpzdhjwpl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gcvrecsfc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gfzhvavpy.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gcmfpvxph.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gkngsburj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/ggeriexgl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbcwfawcn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gnzgjlxpy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gwvzfocht.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/grtuyjrsb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gceuxyjpl.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/glkgvfbxo.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gsifgdpye.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/grcvqeffs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/ggtzibgbh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/grfhzultz.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gyrktvutr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gkbwxiaws.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gwprkrdgg.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gisgosiem.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gxnbouulh.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/ghqlgppys.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gzwhyicqc.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gfziaihne.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gyrknekgp.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gdmzfzxng.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/ghulufonf.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gdsbjspdi.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gxndviktj.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/goejhabta.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/grgynmkof.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gedisbpfe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gapjciflq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/ghoveydcw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gwksuidju.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gzwmedgax.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gyyeyihvv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/goczxbbbi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gbwrnbahd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gkvnhmpww.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/giuwwjaod.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gibqohbwy.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gfxsxduvu.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gmjnldylp.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gyphzctca.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gexujvmik.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/golknvohy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gymjqankr.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gwgbxdojx.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gtcohbqtj.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gdrxujudq.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gcclaqabs.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gsdvpiulu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/ggbpqzdgk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gqulzvlav.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gcevfrecd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gbyrmxfnf.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gaagjntkh.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gwfaapwyx.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/glfhtgsfm.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/growdlpur.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/guttrczah.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gdxyraeol.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gtyhvsnam.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gosutdymt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gksjrvctw.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/glcrbiyxj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gzzigsywx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gjvmoqnzr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpipvqvgc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gixvhvcdy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gphpbnhzg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/ghrytlick.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/guqipcfwi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/ggzutexei.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gwjxivxht.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gpndlfgbk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/ghshbkoeq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gcjndsyxa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gmptmycks.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gjnoghziy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gdkmlmjyv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gqfosdhsb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gixevshdz.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gmrizpkrj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glmudmdso.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/gohihfpio.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gklqinmap.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gcudzuskc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gmpxouiif.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdqmragxk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gwceukegd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gurahjiqt.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/giohqgkri.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gxuuvquey.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/goysqmzoi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/goiegihmc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gkqjnauvl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gzplvydat.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gnkgtkarq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gckfgnbqg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gckdyfjvc.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gkjphcbav.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gvzcidlca.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gfijwinqk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gvexitduz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gyccwxypu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gadwyjhzk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gxemkjonv.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gijouyufm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gqautivnh.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/ggecgzftm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gqttrarsc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/glngtgaol.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gjbiykwpq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gcwuwffzn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gtlbdbgag.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/glxsjuzrv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gaewbojwn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gtwrphwwa.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gfnzwudvo.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gophjujot.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gfavkyzwp.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gmlbxoaju.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/geaevtfmd.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/ghuknevop.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/ganjhkxnc.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gjrllnhfz.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gycrmkuef.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gjxjocsav.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gmqajirxk.sHtML


<!-- 参考信息 -->