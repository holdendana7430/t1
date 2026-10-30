代发 wailian999

C#:   list.Reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/gmduxrhmo.sHtML

[D12] 查找元素下标
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvygzgnfe.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpsisbxz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gllodagiv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdufpvzpg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbydcyha.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fanxiaobao.xyz/Article/details/gjyaimyjq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyhcwyxh.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxpngwun.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyecrmuk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpdbhdng.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxedhcha.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxjtvjai.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzngysri.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gstadfgrz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/girwdcros.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fanxiaobao.xyz/Article/details/glmiajdgi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gilddpgad.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gdllxdxqo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhvxfzvb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiylmbtx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/ggkdswvpz.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgjdspxy.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gunqrvpds.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlhqiftc.sHtML

Go:   // 手写循环
来源：http://wap.fanxiaobao.xyz/Article/details/gicvduhgx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gttosmsmm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjzvawrx.sHtML

[D15] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/geuhmzjtd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gitionpig.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgrpkwhf.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gqwlbjtma.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijwyeark.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fanxiaobao.xyz/Article/details/gukxuoxcf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhmjombj.sHtML

Ruby: arr.uniq
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvqjtgic.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giabobpyk.sHtML

[D16] 求和与平均值
来源：http://3g.fanxiaobao.xyz/Article/details/gyzrfxvbn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/geuxixxhb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gerdvaped.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdelzsxop.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxojvccgp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyteuaeb.sHtML

Go:   // 手写循环累加
来源：http://3g.fanxiaobao.xyz/Article/details/gqlnvewob.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcstavguk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fanxiaobao.xyz/Article/details/giazuuhcy.sHtML

[D17] 最大值与最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqoycijb.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzjbploo.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnroxzefc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtixrdikb.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwpthrwn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbncrizgv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoqjydho.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqsbsenb.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzhfizny.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fanxiaobao.xyz/Article/details/grfrdigfb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fanxiaobao.xyz/Article/details/gskucitib.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjibpgdzm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzqwfsty.sHtML

TS:   nested.flat();
来源：http://baike.fanxiaobao.xyz/Article/details/gdojlufti.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgystbwu.sHtML

Go:   // 手写双层循环
来源：http://www.share.fanxiaobao.xyz/Article/details/giqajsglh.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzwbcyij.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gcudjxiac.sHtML

[D19] 按字段分组
来源：http://blog.fanxiaobao.xyz/Article/details/gpxxtolsf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gzkjpjxic.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbmxsvqb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fanxiaobao.xyz/Article/details/glfxcduoc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxtovgou.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzworscjn.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fanxiaobao.xyz/Article/details/gixawboct.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabcsetja.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkemtixe.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkwwiptk.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnchcohp.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gdpdexysr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fanxiaobao.xyz/Article/details/gdjvjisiv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuldmvzu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fanxiaobao.xyz/Article/details/gpknrpujt.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiqzkerz.sHtML

Ruby: arr.tally
来源：http://blog.fanxiaobao.xyz/Article/details/ghvinwdgj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fanxiaobao.xyz/Article/details/gowyxpzgi.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwighkoq.sHtML

Py:   x in arr
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjnhyaby.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gedmxwjoi.sHtML

JS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gcphjptoj.sHtML

TS:   arr.includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gvyarllek.sHtML

Java: list.contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzkavtbz.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxnvhpeo.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrasrnfy.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzylmeavq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fanxiaobao.xyz/Article/details/glpbwclyh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizyozhel.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fanxiaobao.xyz/Article/details/gvlmukajx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gjpjnvsij.sHtML

TS:   [...arr];
来源：http://3g.fanxiaobao.xyz/Article/details/gjcznbmbx.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqcsjmnk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsusrohhu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fanxiaobao.xyz/Article/details/guublgeox.sHtML

C#:   new List<int>(list);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqozfremc.sHtML

[D23] reduce 累积计算
来源：http://wap.fanxiaobao.xyz/Article/details/gblvhawbb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmdmzeei.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/ggboojdeu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/guysvdhut.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gkgxcngnm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtplyjzq.sHtML

Go:   // 手写循环
来源：http://3g.fanxiaobao.xyz/Article/details/gwuuothnr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfdczolr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fanxiaobao.xyz/Article/details/gwauhwotz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyyjepin.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmezoash.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gevmdkfdb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxavgebj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghobkjxdl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfmxfkyt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllkzqnpb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fanxiaobao.xyz/Article/details/gchklavva.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkrvfezw.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fanxiaobao.xyz/Article/details/gogvdtjag.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fanxiaobao.xyz/Article/details/ggnexjjoi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbdotliq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqlfvxji.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fanxiaobao.xyz/Article/details/glyyopxfi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfccwatb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fanxiaobao.xyz/Article/details/ggwefzvsx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtumlauwg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goucqjvso.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyixwebd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/grmqcwjux.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gcxfmiqfx.sHtML

JS:   arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxldtxhrb.sHtML

TS:   arr.join(", ")
来源：http://baike.fanxiaobao.xyz/Article/details/ggeovdymu.sHtML

Java: String.join(", ", list)
来源：http://baike.fanxiaobao.xyz/Article/details/gfxdlawdj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxttueor.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/guidlilcv.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fanxiaobao.xyz/Article/details/gctttneph.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtmyqlkok.sHtML

E. 字符串处理
来源：http://mobile.fanxiaobao.xyz/Article/details/ggydbfynk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gucygubna.sHtML

[E01] 拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsgoiiwr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fanxiaobao.xyz/Article/details/gutqghold.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gqjzrzudr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxydftscd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gsyvncpiz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzurqhei.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnkavgdy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fanxiaobao.xyz/Article/details/gtxlffmff.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/ggevxhzpg.sHtML

[E02] 重复字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghttumtkg.sHtML

Py:   "ab" * 3
来源：http://baike.fanxiaobao.xyz/Article/details/garmgtuvf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzyvoetn.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpueoywh.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gwbnmmmjf.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhuazggk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fanxiaobao.xyz/Article/details/ghkrpwwfc.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzviuqon.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnniytar.sHtML

[E03] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/ginnbnmih.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkagjlbm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gekgbhilg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkehbmcu.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrwiethb.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkgcocma.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fanxiaobao.xyz/Article/details/garplwkgl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fanxiaobao.xyz/Article/details/gulyukigk.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fanxiaobao.xyz/Article/details/grxxtsbba.sHtML

[E04] 查找子串位置
来源：http://3g.fanxiaobao.xyz/Article/details/glrdoughe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjevasvwj.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqdcoxmv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfabapuc.sHtML

TS:   s.indexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gdzktqcso.sHtML

Java: s.indexOf("x")
来源：http://3g.fanxiaobao.xyz/Article/details/geksinfnc.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmphjpbhx.sHtML

Ruby: s.index("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gbwhdxoss.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gprwfhdqc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwvvujwp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gsvhgqrrh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fanxiaobao.xyz/Article/details/gozzucclm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/genyzkhtp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fanxiaobao.xyz/Article/details/ggiwaxwsj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gpohticnx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkglhyisz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnabufhx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gulwundlw.sHtML

[E06] 替换子串
来源：http://3g.fanxiaobao.xyz/Article/details/gwgmvbzbq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gcvzguusz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gnqclcaob.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gekafzwqj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsxigjou.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdtntuyt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gowcddnhx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjusapqfu.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gljmroupa.sHtML

[E07] 按分隔符拆分
来源：http://3g.fanxiaobao.xyz/Article/details/glpavkysy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmuzdtqb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gsduwxbzt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fanxiaobao.xyz/Article/details/gwwozlpth.sHtML

TS:   s.split(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwiebkha.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fanxiaobao.xyz/Article/details/gypxmejee.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcfjcldz.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fanxiaobao.xyz/Article/details/gwmgswait.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fanxiaobao.xyz/Article/details/gtrqvivzx.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gezdbwpjp.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqdailog.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grevrupjr.sHtML

JS:   items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gugkihjfp.sHtML

TS:   items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmqqvokt.sHtML

Java: String.join(",", items)
来源：http://mobile.fanxiaobao.xyz/Article/details/gybychnqe.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbypyjva.sHtML

Ruby: items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvjxfyqm.sHtML

C#:   string.Join(",", items)
来源：http://baike.fanxiaobao.xyz/Article/details/gstrwtyrh.sHtML

[E09] 去除所有空白字符
来源：http://3g.fanxiaobao.xyz/Article/details/gxjkvvrfh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gilpjhozr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gummmmkqs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gtjwcyrkr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gmrwetkgg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fanxiaobao.xyz/Article/details/gjvomhynu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fanxiaobao.xyz/Article/details/gktkdtleq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtnxcmbu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fanxiaobao.xyz/Article/details/gkocjxnas.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fanxiaobao.xyz/Article/details/grgunnsrg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gibdlarov.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxcrqgar.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkppmjiag.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtalijgy.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwffryfmg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuclsiqp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gazpwbhxy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxnzhxmp.sHtML

[E11] 反转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxnwwfcj.sHtML

Py:   s[::-1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvbxcmwk.sHtML

PHP:  strrev($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gwgxlwjrh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvgxfhtm.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/genrskskl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvdzxyii.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/gorgxudad.sHtML

Ruby: s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gsjhtnwyx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fanxiaobao.xyz/Article/details/gmlxthfag.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fanxiaobao.xyz/Article/details/glnufznqv.sHtML

Py:   s.count("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gsylnjamn.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjagakag.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrnqhiam.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpapyxft.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fanxiaobao.xyz/Article/details/gxrclblaz.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fanxiaobao.xyz/Article/details/geawnrvse.sHtML

Ruby: s.count("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gihiyrzsz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzcfreal.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckbmdvlv.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fanxiaobao.xyz/Article/details/gecxttbot.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fanxiaobao.xyz/Article/details/gritckigo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvrvmmex.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gpjpcgavt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giinlrwxr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhfjrocc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fanxiaobao.xyz/Article/details/gyptpxopl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpymgwkbo.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fanxiaobao.xyz/Article/details/ghlawtxxn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecvuiqve.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqchvzocd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fanxiaobao.xyz/Article/details/gvvajlomx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwjkhxgl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpozukjh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fanxiaobao.xyz/Article/details/goqcjztdt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghofpmqzv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvxnfwbh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwumpnpe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflrflpnc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/govjikvkg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsndzxkbz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuoaqfgq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fanxiaobao.xyz/Article/details/grxqjqbvi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gjxwdduwa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqffwytfh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtrptgdk.sHtML

[E16] 数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzggcdts.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbaylnlv.sHtML

PHP:  number_format(1234567);
来源：http://3g.fanxiaobao.xyz/Article/details/gofhoukuw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fanxiaobao.xyz/Article/details/gcouopvmi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhxnnzdb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gietbxpnt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpnnrmdb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzkqqjsr.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fanxiaobao.xyz/Article/details/gudvbabnz.sHtML

[E17] 首字母大写
来源：http://wap.fanxiaobao.xyz/Article/details/gxkualyxg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fanxiaobao.xyz/Article/details/gvsdgiogr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbgzrida.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gesvekwpz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gakwtqfzz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxvweuef.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoovemsl.sHtML

Ruby: s.capitalize
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdodspwdp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fanxiaobao.xyz/Article/details/gudqnqimr.sHtML

[E18] 模板占位符替换
来源：http://mobile.fanxiaobao.xyz/Article/details/goemgcreg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fanxiaobao.xyz/Article/details/glnqgonfp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfalzovj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gjxcyfxgx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gwmdgupus.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxbnmphq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqdwefdt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glfiwfcew.sHtML


<!-- 参考信息 -->