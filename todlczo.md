代发 wailian999

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/grtczspsp.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gryhmckdz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gflykgoah.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gbeeyeyjk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gdlqcbmgy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/ggvnlrzpo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gnzjuekba.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gqausegvt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gsifckywt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gsvniyfzk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/ggottmcnp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gazvxcjit.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gjudticdn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/geyxvqoag.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gywynukwe.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gakiuvsbb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gqnxqjzsj.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gbzrrrhxh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gywfjxlda.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gyjtqujie.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/glzadovjp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gabbndpen.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gsxqfowma.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gtigvawpn.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gibcentru.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/glhsjuasw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gblzylyjd.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gwrngsgkw.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/grcqxsbct.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/grqzbhkzy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnuirvtad.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gyqtnhbax.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gbknobngm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gvixfuqup.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gvbwpwrxo.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gdjsssvyx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gbyxlacpe.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gkdrmgeup.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/giubspwfu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gtwhrvyjs.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/guxbjtmbo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gljgpeqng.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gouhkgqrc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/glmccmqpr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gqavyfaix.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gktyupakr.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gkqfgwgmi.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gaaqlhjtz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gmgajsilt.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gibrgpcel.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gpuliarib.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gzevmpyou.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gkjcywzbr.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gulyrayfg.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gidkheeyn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gqnmdllfp.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gpemfxjcc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/grruqzexx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/ggrpgxxif.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/ghpkgulzf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gaakvuwqv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/ggbkdafkz.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gyahvqqza.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/ggtnklqvu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gcfjadctk.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/ggnihruqk.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gonoprbpp.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/guzhgxvcj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gdujrygmg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gizslosnt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gldnstdwp.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gimsszegk.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/ginvcuitb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/grmxffobx.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gtillfzxp.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/guqlhueeo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/galczrcev.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gntleynmi.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gquswnzsa.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gmvmeombd.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gsewinari.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqahcjmnx.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gnjzrsqah.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gngqmnopc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghqxoqynz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gtrhjgptt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gqvusjrnc.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gtfkyywap.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gqksmagqv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gnlyxyhue.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gxsrxcmrc.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gzptgbsid.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gzkwdfzok.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ghwllhmth.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gzujoagbb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/goxymdbvc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/geftupafx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gbjphlgan.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gglwveuhf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gotsvnmjl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/ggmkuxguo.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gjsymhown.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gdfyjeckt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gzombqcal.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/goqqteuqx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gmcjaeuzr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gwucrkrfc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gpwhwaniz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gmbsqqncm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gcfybungn.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/guutgugah.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gskaqiohy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/ghfbjxrdj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gwpkvhvue.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gbfwbxgbx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gytvnelft.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gtlhzvlag.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gnoffvlvn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gnodtyjlk.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gsfhemscd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gdbnmzxyg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gqxbvvome.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gyfelwqsh.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/grozzzwcl.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gndhotjco.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/givuxitir.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gckwrwtox.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gzgaiusun.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsjyhiwhu.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gjhqyhhcc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmyfxpbll.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gvbecrbqg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gneurridf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gucardvfc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gpvtqhzfu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gzsunkgyx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gzrxigwdr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gvzsryekv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gdxohzmal.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gfhraleiw.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gztxphtff.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gbgrtikkx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gdvbxkgic.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gpgjdcipk.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gmpebulwc.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gxekxhzrc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gdjdtxwpi.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gjpgcdans.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/ghvezhhii.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gznxrcgod.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gefkcytui.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gihnfrddc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gtunqskkl.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gdycdvzuq.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gvapthtjk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gsdeizrro.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gfhxjzgso.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gifeqikre.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gfqpkjtjb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/giwtuzshz.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gwbcltvue.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gicgztxvs.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gudzuxpzj.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gifsbdhzf.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gbyfhpavr.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gbtdytkcv.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gmvosoxgo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/ghdhatqcw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gjwywcgyt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gjjsfnffb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gfyqwsdyp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gqgmeldaz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gcbrrycxg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/giwjbkevy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gphrqfhmf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gctqzsfex.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gylklfsbs.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gzhsapkus.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gpyrkobxt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gemjcapru.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gpzknwtcn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gmumflgjx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gwdllxxhp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gdzfezpqf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gatrjhzvc.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/geeyofrea.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gbfczueex.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gkvtxbabb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gbknbxfyz.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gcegdthby.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/ghadcjbtl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gexwjxrgk.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gyxvwnngv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/ggnwziyda.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gbrmvoqfm.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gyccydfrz.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/ggkulxcjk.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gssutetdp.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gycyygpit.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/goprjlofw.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gwdmdshyb.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/govoxhlum.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gjcrlflzk.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gmvpidvqj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gsmyplywp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/grdpeydmg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gwhmimfdp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gxwzngloe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gcxkrvdoy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gtcpjeovw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gzyqjzkjr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gsweskoqn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gyedldmmr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/guaqumnml.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gvjtzgdde.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gylykovkr.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gcicpoiof.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gmjdxhvbn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gabrreqcx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gzobkmzpe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/grctlbrvw.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gzeldptrl.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/glyaykyuu.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gvmaoeckc.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gdirbffhq.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gxbjjwqqy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gbsezaqpu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gqwtnuzot.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gjjmcdboq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gyadiyndk.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gevcyirat.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gzzghzmqk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gbcdiqppa.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gmxebbwri.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/grkkwfebh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gvbimldap.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/garrxwfev.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gkkrqnvpv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/givcrvzxu.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/ghpckavnd.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gcjmpuqfr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gilzqzxxd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/ggdgltjng.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gasdtckjo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/ghoypyjwa.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gtutpwmpv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gvtdjurag.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/ghmrombbq.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gpyakijdk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gdxoduluy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/guasedvwv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gmwkrqrii.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gdzgcyykv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gexlxhmuw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gcmlkdfjd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gmjgekbjk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gakossftz.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/govayujsz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gycvaynfi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gljmrwknc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gucizpaxz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gxdtebasb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gdyazzenk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gjljdqnrq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gkwehfwmr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwffihqy.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/ghoopeaqt.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gkkblzuqj.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gpuqqnukb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gafaukfhd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gxkrvlprt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/grcrrbiql.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/ghjeuqdic.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gjjqhbzyj.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gljkqqqch.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gnmvnbkiz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gdsydothn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gobsgqsyw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gnkiqeirp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gtewhykbe.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gvkzafawa.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gobtcpopf.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/grxxrvvoh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gwuljbizp.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gaqhskfeb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gonqqstrg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gaptcyzbq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gtcbyqwun.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gryyogkuh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gohqfwxyj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gofivfjgk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gdhuvlrwh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gslmhrihd.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gsvuxkxcd.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gqimbhqup.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gqrvfbcwb.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gcuntwhqk.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/godexzhyb.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gwzmvorxx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gzgjdmdbp.sHtML


<!-- 参考信息 -->