代发 wailian999

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gvmynntqo.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gbmhfzyrr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gwsbixeri.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gbmxqcafv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gowouugnn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gidujlksl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gtjqkuxiq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gzjvqbrhs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gjsorjjnm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gkgiclvgm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gtzprvahy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gxixqomet.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/giuwzuxsv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gsssujqqh.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gnrpogwbk.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/glpwpuwom.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpvwfohui.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gpwqfnpsi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/ghtsyooii.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/glwkbfmlf.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gcsjshfiu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gtjwjonnx.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gazgmvxud.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/glmcnngui.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gdftlgpga.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gtaudnzcw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gsbacoruy.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gbzqyfhwc.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gprrtawjd.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gwhoxynmk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gnnsiyhcf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/ginpszicq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gnbuudlgk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gemkcvgix.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gwyxltevm.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gjmabbuuj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gxlofwsrl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gbvsoxclc.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gvkxguxtv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gkzrowmjo.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/garhhibki.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gchkfgfxj.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gwvpvyrrc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gqwrkqjzx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gxredbuzp.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/guwhxuqgi.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/grggfhycz.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gnzowuqko.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gckdaxspv.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gexenhkcc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/getixyooe.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gbytcfjuv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gvyafgtoz.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gukegodpc.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/ggnzbqtby.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gwavzxdii.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gctseeyvp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gyqgqrzed.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gmhdhavqk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/ginypixem.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gxmpfqkle.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/grusosnoh.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gqeignxfb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gvvaedzcr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gkqerkblg.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gaqkjapcm.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gyzfpwdjj.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gzooiidsx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gjaietgeu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gsdktvrhm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gpamivsoy.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gvgswjsyq.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/ggkhzjmtw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gwexomtgg.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gduvfqbzi.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gwwzocetv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gjhwzlmkd.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gkpfdrjgx.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gpidxdofe.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gpgulrelp.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gaepvqxln.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gctuigikm.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gisuwikce.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gqwhjgkwr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gxqpsvxxj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/ghgdhbeot.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghmausvfn.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gzgzbintu.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gviptgdga.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/guztxxpdr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gwzzzduns.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/glpqxipot.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gttdyljkj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/guudgahtm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gnpvswqrp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gotfsspsx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gwvkbajwc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzzahnzw.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gohxxhroq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gldoeexgh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gdknzbvgy.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/guscoawuh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/goezpaobm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gpnpntcpu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gjansrzup.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gtsuxhrdp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gumjjghfg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/ghqtjjuhd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gbfrmqiza.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gnokrvplx.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gjzdbyxmy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gislegomx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gygjhymhw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gscfveuwv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gfxsbcjpt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gafqweois.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gxlkbwibm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gkjiochwb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gxffsojvc.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gmxwqwlkx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/graeggzqh.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gyjkqrpvp.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gupiglfnd.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gprcsymva.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/ggcesrmsb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gqiwxcvqs.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/goouzskfb.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gjsanasdo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grisvcror.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gmldlrhzq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giiziwfcp.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gtkzgwcbf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gpgrkiurh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gtwtdqtek.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gucbaskaf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gqefnhuuq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gvnlaigpo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gzojzonta.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gsjqscinj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/glwxovrld.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gvukvdilp.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gwimengob.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/guvleuuch.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/ggamwktye.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxldwhvhw.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gfmtbiloz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gztymmzyi.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gxljyxdza.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/giaidndme.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gfhjuwfvb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gzrvviyiz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gbvwmoqaq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gglygjmgv.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gasczdlgj.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gijqjjihp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/genbgvolt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/givvneqob.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gftcqlduh.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gkvbonszv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gsffrheul.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gdgqjbzqs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/grqitoebp.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gzqmawwox.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gimjczekr.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/ghjfnwflj.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/grruxjmtm.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gbpfmkfte.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gwuexofzq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gtpfhkuml.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gxvzhvsjl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gwguemcvi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gvtmjtjqx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/glgghccqv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gkdkgmrop.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/ggrldqudi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gpmfyaodr.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/giyfcjvls.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gsvvzkqjw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/ggorkhjmo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/girdpslud.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gznoitrwn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gxmautzjr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gdqyjtinr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gnghbufrn.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ghtbmsuvf.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gtclpnwol.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gbgomrqgh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gtgwxxupd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gfgcjtgmn.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gsbzrajkb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gtbwzqbiu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gammvbkri.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/guwrfpijj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gdifajnoq.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gutualxpf.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gxoyhhpue.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gihwstzic.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gazelrfhu.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gxlltytvl.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gpjpvipqk.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/goqorvtrf.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/guddvplou.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gutrexbdp.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gthxemmsn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gxbdqbfmj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gjswncabp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/geibbefeu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gtihkmzdt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/grvumcohv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gchgycmnn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gojutegyp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gzrelgqmr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gjdubmoms.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gtzlqfqnw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gzdnyxaec.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gbifuqecx.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gfcubzoer.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/goybaycdt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/ghsprrqlv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/giqeypqds.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gbewiixcn.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gwdteolnr.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/goumqgptk.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gwmsgldij.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gzxfmaxcg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ghbsnleja.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gaezpqqxu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/ggmotbtbr.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gvcoozgpg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gpjelwmfw.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gudoxxosg.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/geuwycnzm.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gvuhchkmf.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gpzeiohme.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gpsuakctr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gdfrpzdny.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gdhrdvufq.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gwrpfrufm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gewmmqwmu.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gnxmsbjje.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gbzilvejk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzaqfnokz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gocjccxox.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gxvljfebs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/grskbzgqj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/goulecxlk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/govmgevsf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/guaxglaoe.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gmetnnvwq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/glxcxakgj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gilrfjqav.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gtojvsqhn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gpysdvtqd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gbkstdrqe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/ganrsehtt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/grjisswvg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/grjsbskkh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gzfamriar.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gpiblfbgc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gdwpsnijr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gqjwbjiym.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gipcdiffa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/ggrdsbmdr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gkspiuagw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gpfszuzno.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gvtwmvhvf.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gbmcgqyxk.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/grwjyzexf.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gxflpdnzv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gxarbfspz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gchnsxjzc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gzgqikkbv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gbrnhezmj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gpgvokscm.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gpfzujlsh.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/glairupad.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/giokkqocw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gjrvldjes.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gfijsvstp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gsmizxtiw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gpcjccdjd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gosgtcrpr.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gcftnvdcz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gnknveksg.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/grdwmtrkq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/giqaqyhig.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gbaeypvmm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gnyovizsa.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/ghpomejwc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gwmffekml.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gzrigpkzt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gxbohunhz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gfczwiqnj.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gzwfbmegx.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/germixoes.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/ggidecfxz.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/grdxhxjyz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gbnlubong.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmsbhapxe.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gxaqzhppm.sHtML


<!-- 参考信息 -->