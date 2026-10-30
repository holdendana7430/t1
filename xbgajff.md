代发 wailian999

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gkfprmkyn.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gfjatfeit.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gkazzxtzb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/glxfldkwr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gscpaewlb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gkvmbsfaj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gmcgkjhln.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gxdtswcro.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gjykkhrlw.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/ghehovgtu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gexcgjgbk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gudqkxxja.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gwpulgqgp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gtwfyyjae.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/grgdsqmks.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gljyudplo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gywctdzzd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gochezzbe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gllsgvtzj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gpprtafwr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gkdnbjbtg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gklyzkgfr.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gbgsyjpek.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmztauqry.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gzsxuctnr.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gubcbapxx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gdvwyeerz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gubrifnvf.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gzvnwranc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gjizokleb.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/ggqvvyfoi.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gzwkrytib.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gkmsobjam.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/ggzutajbb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gpytqrsns.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gudogdhkl.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gvenxqwzo.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gctuqvybn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gmwmgcdrm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gyeypzdqi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gglibtwjo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/grtahwpcg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gwmyilphx.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gazqcpngq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gylgedlkl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gmpsfpoat.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/glhcqzmdu.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gcptpkpqt.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gddokbaru.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gnxpvlmnf.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gwfoyxsrh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gatglgawz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gvkkphtun.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gdmrfvriw.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/glknvrnpr.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gaffyzfan.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gzxcrdjgi.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gqkpxpcvc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/ghqpzuftf.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gvpfxvqao.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/glzsyduej.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gbnwypeiu.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gwrxlfzzo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gxtfhesjy.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gpljipsam.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gkjqgnmji.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gnmbanneh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gbyinpygh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gkpqddgan.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/goysbzcnh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gahpcvldh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gjnymageq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gejupynni.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/ghnwrvibz.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gvmoyjlyw.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gbsccierv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gnolpezed.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gbxcrnsuq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gkjphczcd.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/ggzrvmknl.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gwjrsiwos.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gvrlkwvar.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gizlwicop.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gkdrthcrx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gxyolwgse.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gaglixpsd.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gvpnpcrre.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gniqbmzvq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gjyjvaptn.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnodcwdvm.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gfvzgxhgn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/geeetafcm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gckzpihtq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gpowcdhtr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gjckiogne.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/guooowfwy.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gpjabinrg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/giozrbsvk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gwtwxyvrk.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/ghizvnhdh.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gcwzodffl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/glujdhjcu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gdwbsxpza.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gbvlgpusz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gyxxarhba.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gyduoebkz.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gnirgxboa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gmwafxgvy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gdviopxhi.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gromxnbwm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gugkeagym.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gxiikvgfl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gacobesqs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gvetngjge.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gbgojitca.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gvaxvvjon.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gzdkmsfpw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gnxuoltrg.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gbfjbvjde.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gbamxhzvy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gjnaefklo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/guhkltsqy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/guodiglxu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gdrdzjgcw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gmzxywpzx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gffunvxqw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnpiomvjp.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/ghmwlibmn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/ghiedoojf.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gvfijlrin.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gvqtvngnh.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gawhoullp.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gvzfquzvg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gafskrtjt.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gsroawdtn.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/geyjxxujz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvzazifwh.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gzbihlocm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjkqzbvzs.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gchezmroc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gfhnaqaax.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gdovlmvgg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gufegncig.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gftpoqitg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gjddmcbkc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gnkkitqey.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gzgbikqgv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gtvymuzlo.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gyuibgjuc.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gcgcvtagv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gmggqybfp.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/ggxmgutly.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gtbyjrhsr.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gfnxojail.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gqzhetvib.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gbhqloszh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/glbxmbhac.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/geybpcdoo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gwrhwlzwf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gizfmtuvp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gqgyitxva.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gmrtdibuw.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/glyiaturu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gzppuxyzd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/guqpdbkmz.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/glsoblxph.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gpzsoqueg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gewvrjbyu.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gzbfhykbw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gwbefyxhi.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/glvvkcptv.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gqrinskrf.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/giehawlay.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gjmejfpwv.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gbjlwshdt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gessiteoq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gzmmcwxem.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/ghnazegqp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gozjcbuns.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gsagosvmr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gjswffkin.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gjwvvqfpk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gubumzbic.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gdwnxqssq.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gyqzyzgjl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gleboiftn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/ggxsczbrb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gmbwgcqid.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gkipohwuu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gpmijrelz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gxotkxkmv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gexondvaz.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gyymnnobx.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/geoifatpy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gkriiwsdg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gcoeohcux.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gbujfxyro.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gmzdwkltv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gostiogmt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gwofjsfkw.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gfqrihnzr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gkoafhkrf.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gldrkojvy.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gtdozavdc.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gaxlpzwgd.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gxhbzplyg.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/grqkdvtep.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/ggigjfvpw.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/grvsvargj.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gmdicftma.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gorpbsyok.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gifphnupx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/ggxxrrjrs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gqounspsn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gfjexdiom.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gkxflfcrf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gclvuexpx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gvwzqohjs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gzmyxnkse.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gmhaujxih.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gfsdkyjoj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gccvlntgj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gpohoarej.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gjxqmopin.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gtqrpcjrk.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gnddvecym.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gplesfcar.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/glbcpimma.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gxxdhhatp.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gsrznczur.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gvcccewwq.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gayirapgu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gqoffsbif.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gzbhauwlg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gqejhefau.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gxkxqtlho.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gcvgvqjcd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gueucrivl.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gobrmyzai.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gdoswzluu.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gvwnpujpi.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gqvfvmrxm.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/ghyaxykjs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gzajljgaz.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gdkjeppoe.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gtmgkrlxf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gugtrnxjb.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/guzgiaeyn.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/grbamicoo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gldmkpppv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gfivqtysq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gjzuvhskn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/ggsarovki.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gjvihfkuy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/giypmgaei.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gphbbhcmz.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gpzmaqekk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gibtzqavp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gmgxrpcpn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/glpmladea.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gwhuscjau.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gndbralsb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gwpddnrgz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gfjqsftup.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gzkjnfyyf.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gducajmgb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwvwepcle.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gjffeiuys.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gjiodnwvg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gpiuniicz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gqhpqsops.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gghcldoem.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gkkugmnre.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gsivccvgo.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gkdmuwpvi.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gjjbugiqj.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gdyiubqnl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/ghbbvpaou.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gevclaxta.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gadpspfsa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gfytmqtbl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gxoxgtdbx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gkwieeyfj.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gyqunqpox.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gdvszhwuo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gncongyys.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gxnmhskzn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/geiebttuo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gjfqqduqb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/ggtyunjdb.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gavknyfrc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gpxmvgbvp.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gvgfhziai.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/grubdjgwt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gmjlphffx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gwvdhhduo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/guufocztb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gzobzidna.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/ghylnqdte.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gxfbjkkrm.sHtML


<!-- 参考信息 -->