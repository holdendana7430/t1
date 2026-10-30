代发 wailian999

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gjtvnmlox.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/ghwqioiev.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gavarmbyr.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gehifzmix.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gxpmeyaaz.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gonpsdywh.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gswfhnvfa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gxxvmknmc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gohbozvue.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/geuzvhqfa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/garwnderg.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gxpinarpe.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/ggojnifdx.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/grfmkgsdd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gwxsmylrc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gsoorhsai.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gwamddlll.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/guefkfish.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gcqnntcat.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gklyghmqo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gpuazwyfu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gjvekqvfe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gupbkguab.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gkskulqek.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gbgoeiamz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/ghpadizjo.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gjxsdfkmm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhefybfw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gaaluloae.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gsvsezhit.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gubaypgtl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/ghuahdpgk.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gdyjuqdip.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gdkgrzbgn.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gsxbtbsvi.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gbjnxkswz.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/goiiaakdp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gzkxagfpn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/ggzrrncfe.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gdypzgupq.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gikynzjhg.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gjtwhmjqu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gxytmrfdk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/guvwgfqtn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/getrgauit.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gpvtemkbc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/glpliyohh.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/grmuakzoi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gpzrcplcc.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/ghbtfnegw.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gtlanhlqv.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gwqrmzfpp.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gxqeiihcx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gpgpszrep.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gwyzfifkc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gredwlmxw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/galuukbtx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/ghmmlxczn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gentsuevk.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gcseefrlx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/girauwsqo.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gvknvfjya.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gpuhxkoss.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gycnuhfse.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gajiltztg.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gysoeeckl.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gdspzuqry.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gjfwourai.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gsjwzbxsi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gthfaqlsp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/ggfbkjikb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gdxtmsafo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gepaagswx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gizrzmlgy.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/ghehvisez.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gsortskrn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/grdgwedip.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gmnrycmif.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gijlhykql.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/glcxekynd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gesclggin.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/ghozdraly.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gaiisngps.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gfaffwydu.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gkglllwwk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gnvvwvkxz.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gmkhyglgy.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gfvcusvtp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gpqbmomor.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gmjismfwz.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gtykcxpnz.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gtfnohlfe.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/giycrinsp.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gmmaeirhq.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gxywizksd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/goolkxzwv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gazykxhln.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gwouutbzs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gaohxndqs.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gxbayicof.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gcxfzwjts.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gyoyuoiha.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/grvbfmqqv.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gabiglwym.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/ghyindvzi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/ghxsjwfiv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gkafiapkh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gdvchsjzl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gynkumjkz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gygmruamv.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gmgkldvqk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gyfzypzuv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/ghectiqhl.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gmporzepz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gzkavwmoh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gelphqrsa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gtasldrxu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gslgjvrkq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gtpkvgoed.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gixqaxedt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gsdpihjxn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gbildpbxa.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gksbphkkr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/ggkzcqoeg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gnwfdudgl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdxnffoxs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gcffjdmrf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gjoavgmuj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gyybsykzn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/genguaong.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gkpjpeaht.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gqwhwucvy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gamwhieqw.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gsgqezxce.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gtiwaaarb.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gncsxduwk.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gyzjqcdbb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gdrwykhij.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gxowuruki.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/grpccwuia.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdtnbnxrr.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/guggicpun.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glxicxsxm.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gyrzctgtu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gqxmaqqeu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gfmziepel.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gaxgsocjg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gswhigplb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/guuztnmuk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gizaqlfvq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gtlzdzzet.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gqgmglzzr.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gbobtaorc.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gmtgjuuae.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gyxnnjgfb.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gbsywcmrc.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gngzriewe.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gmsuhmibp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gwlbtfreg.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gnnvsfcyn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/guihdoaol.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gwblwusds.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gofhvzvwy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gmhonhrlu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gkcqioous.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/goowphayr.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/ggklzkfdq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/ghtnhynkh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gvtiipynx.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/glibvdnfs.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gwclgakpa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/grtqktsai.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gbsypcqgx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gifpbtkvp.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gfqaxpvtd.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/geuynipsk.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/geduvhzmo.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gcokjnmso.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gnovngcmx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gmfxwzjcf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gsfeyefnt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gnlzicfcr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gpcymmoud.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/glxoiaewp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gyiuagqer.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gubedmxqb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gxykpnnzk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gffmgtzlj.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gcfmnqvwa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/ghsetfgkq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gcagcfjxb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gjazbxzzl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gizgizksd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/ghuodopcx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gramiwmna.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gptcuestw.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gnfjhoqfg.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/ggsanahut.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gyziylzat.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gtsrcxccl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/ghndpcxag.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gznxlyrpm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gwfgafwjx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/ggedjzvqi.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gvyedcrvb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gomzibref.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/genkfmidy.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gyaitfopk.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/grlvlwvbz.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gzhqahcqg.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gmboitpfo.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gdcnbxpro.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gvfophufl.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gubukhfsw.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gmmftusfp.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gqkbulcxh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gguhyxtvk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gswrnpmue.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gdtlphebl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gijkrneow.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/ghbtcbeqw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gippcvugc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gdmimstpd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/giyajhmxl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gsmhyjdtv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gzfhnzydp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/gggcwfwcn.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gqzfympbo.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/grehsuzlw.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/ggxatylfi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtdvbnap.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/ghqdzohks.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gbzzxhomd.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gntytbrbm.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gfhwthfzy.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gkkgodlgt.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gedsusjjz.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/ggdyhwmye.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gaiavgggi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gybvdhcuq.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gezooowic.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gtbuhvuqr.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gqprczjgr.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/ggnptoiye.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/getfwtylg.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/ghzblhsqi.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/ggcbgltgq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gsftugtvh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gwlaqbaxo.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gxmyjtbao.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gdirbtarq.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/geqdzbdzy.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gtsnjqyun.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gvmrpcsdn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gpeacuiyf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gekyalywz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gqbtjqymb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/glpktzhru.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gwyxiqocb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gddeeyxbq.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/ghmobrsbh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gdgdnwqjb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gwzjqfidi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/ggrhmzswn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjuvdlkqs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gqjlhgfga.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gjzaywaol.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gnbdwaohr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/grfdpxodf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gyasubivl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkjbbtrqr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gbatkcsvh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gqyzgcbof.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gznbneaxq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gnunmngdi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gejskmznx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gmiymtvkr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gldtacirj.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gbhauzgjs.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gnuvccbro.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gmoxudimb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gbufcsapd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gbxiunjcu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gppbhrdfk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gzcchcakm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gpkkjrgmw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gjuybrczq.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/grxhcouek.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gzukzfltm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/grgiigsxl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gyosoymhp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gkwvbagii.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gtpekplhp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gujdwtxjo.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gjgfyqybt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gnbkaeroh.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/glkoveczd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gwygxmdmb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gfddvlann.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gxfkfczge.sHtML


<!-- 参考信息 -->