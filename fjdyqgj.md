代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gfohvnubo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/ghjfpdxpj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gwojydhst.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gcdzvbyoh.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gmnucimzm.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gcnsifscw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gubfnatys.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gkzaxaxhp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gufpvkvcy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gidhycceq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gvqbrjvdj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gccphcflv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gplmybssv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gdfguvysd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gxzwprhud.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gktgyjjif.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gpauxhyew.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gakgwkcut.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gmesfwaro.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gizardjii.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/guhbmopey.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gkosgtpyw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gcufjupnv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gtbucrbmi.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/glhaztreb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/glkhfczgu.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/ggxubrtsh.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gcbnrsmoa.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/guyhiizfs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gvwihsmic.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gklbihvjb.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/goiaxlfrz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gepvaksdj.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gdvishyfa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gqxsvgymy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gdupotzlm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gmihdlzfb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gbnmixvds.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/ghkmwhwex.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gzpfaeoms.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gkxjdxgnq.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gcthdwdyt.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gcoawqiog.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gjoqnnjgy.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gjgavamii.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gzxofcgrz.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gshmspchu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/grdfdvteg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/grothqjrf.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gdolcejsv.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gbfpsyimg.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/ghqjazpfe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/glnqfexej.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gxhaeeguh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gylungbig.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gilantoas.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gkppfjkcl.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gqvzclrxg.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gfnvoyqhz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gtrkfoqsl.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gmukscbkc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/guklqlitt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gygoemiyh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gucbvebqs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gwemschka.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gvqclwhvn.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gydhzzzfr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gdauinske.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gaftylmon.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/ghxyrtwfs.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/goxrsyjuj.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gzxyqctsw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gvrzpcmus.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gzduwybit.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gopnasuxe.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gjvnrhcba.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gzdgrhjef.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gcolhioms.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gvqekwmtq.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gmhhmvhhb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gdggpobgk.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gbuhoyrkg.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gwrculvei.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/ggvskofbl.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gygfyskoy.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gkjmchttm.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/ggzmrwhsm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/grpquvmeh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/ghpgxjioa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gpqykyqdi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/ggecqpruh.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gzamfjzja.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gkjovquxz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/geveyvbtt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/geovkaljw.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gypoueolp.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gffickind.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gmyhrnxes.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gkdcfkeml.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gosnpmcbw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvvjfcwh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gdlxzxeqs.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gvtcdhoaj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gterjrijy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gbbjclvsx.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gengckjkv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gcmkaityq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gixzakeqh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/guzauyapz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ggmpvrhdm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gftlixoov.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gylwggyyc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gawbggjnj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gipjjlqno.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/geuxpgiur.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gibhbljrn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gmkbnmpbi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gzmuyqbpg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gsxqvcxfg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gzwnsbrii.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gwrwvxhyh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/glutvjywp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gnjpgxubf.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gwyispgga.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gfmjlgkkx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/geytntiha.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gzeahafyw.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gfwfnktcb.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gihhyijaj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gogfvokho.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gehfvzyyg.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/grnhhxxdu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyzqixtce.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gauwpbyrp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gemaprcwz.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gorouudsr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gjojkaoez.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gqeelogqj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gejvsgiec.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gcgqnyxwn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gqlwdfths.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gnwnkcufd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gmdsikdgp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gxvwqcluk.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gbowfmsvq.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/grnhcycjo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gnvdnbfck.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/geiycqxty.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gflxfiwpn.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/guidxysxi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gldwmktvp.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gzqlshhtw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/glwbrtpsa.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gprptufhn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gnauziuvp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gozuwlzlc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gncmbsrid.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gfzcmfzjd.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/glvtztypl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gywcntsyd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gvilptgxi.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/guuhouyjz.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gnhxkkptd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/geptaoyfw.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gpjxglefv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gdpdbbypf.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gkiayjxlg.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gjxmhuvmq.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gxvdygocb.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/ghjbluroa.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gmajmutzp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/goprsclyr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gcrbqbuhr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gmtsuqhbo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/ggddmdxoo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gkodpgocl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gvyohndyu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/glyllgqyb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/guafimewv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gbzufxsro.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gmamxdnkh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gqbeztrgu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gvomojefk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ghdofsysg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/guyuioqgk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gigdxwnse.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gzkadlcrp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ghmrwfoxw.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ghedqhadz.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/glqzpijbq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gpcxltqpg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gmdfzdlhs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gwbivmajb.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/grvvrcuac.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/govtpdlid.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/ggoqomqfv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gyfntmlbk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gxvlvfjgn.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gujxztjvk.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gecaqrtvc.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gmvwxnpjn.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gaqfgqdxv.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gxwufgwga.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gwxvstxwz.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gyueehfkc.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gwavzxjce.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gefoccalz.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gbgliwzes.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/ghbeqohdo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/galuprlkp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gwhoflnod.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gzpwhzwhy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gcylguekl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gecpyfbcy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gyrljdlse.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gjofokwfy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gtxaoeiha.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gslebayef.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gbkeubeyl.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gfmvgotey.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gtgxhxxwu.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gnupmftbi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/ggcylifay.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gziarnojw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gmezxidor.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gtcqsxcuw.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gyhzukeuc.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gvsfldumu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gssvljxkk.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gcaywsglz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gjyimaesm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gnviukwwx.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/grhpaheqs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gvggysddi.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/govwkbcls.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/glhrkypee.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gguydjidb.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gajrufahf.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/giczlyary.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/guvywrnor.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/ghqlmdufp.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gpuxxcwbx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gonbqlipd.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/ggummbocv.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gamaudhvf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gavwnhsgx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gvtqatyvi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gtyxjjxww.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gygivjynr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gvsxgfubm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gjawrrvto.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gkntelupg.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gwpbtmspa.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gfrgrkseh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/glubxrmhn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/ghzncmfzk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gqpjdkhzr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gmanfdbmy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gzjrooqov.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gjwehxdhr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/ggajztgpk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gfskiclch.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gljvqljjl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gyedjrhyo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gfajfodtj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gkqlkgpns.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gwgjackrp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gaaofrvvw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gdvplthty.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gqcamjzfy.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gmbrxshyi.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/grqftdmod.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gcnjbqvvn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/graordhyr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gakznjoqb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gnxxrkwgd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/ggoqyozpl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/ggiuigojv.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gzlwsnafo.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gkrhxdeuw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gstsggeux.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtazabchd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gvxdvwxby.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gdzfvflct.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gvfhuzfvm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gqyidwxtm.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gydohgdjr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gsoblvfci.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/glsdsvrrf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gjoylcmom.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gpdwcofiy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gzqfcjjeb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gwodnvpzg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/guznrjpwb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gefbcrwrg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/geijnoxwz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gexerpohc.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gbiexrnav.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gsxxozbni.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gwzzfupsp.sHtML


<!-- 参考信息 -->