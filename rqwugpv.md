代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gzpmktnxg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/ggplcsivl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gamagsclk.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gsghbxxij.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/giibptrbs.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gzvfkzzth.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gsgnzivlj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gsukpzmvn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/glxdwdrci.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gdrdmucti.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gxcekxfcx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gvfjsaqmg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gronjtiqu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gfflajswg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gexespqvk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gocnstjcw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gxtoevgtc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gosjdqukw.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfkmhlgik.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gmwnkvgxh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gufgdrhhg.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gglvslape.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gmiykbtjn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gplhirjoz.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gcxteljvq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gbpzqewos.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gfwchxzvr.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gdejslznd.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gqhtidzad.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gkknlxali.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/ghhcbvitl.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gagioafsj.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/guuguooct.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gfmiytnne.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfipfvxrn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gxrbibuqp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gscrgkrmw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gapatmfoa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gbglzepqw.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gskixzbgq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gzgbagyfw.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gzcxtksdz.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gvasegpmt.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/grmcthxcb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gwstudwzg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/grsnkgrwq.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gkrkazphm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gujzwoyms.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gbhkfgtvf.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gpevurjfj.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/ggwgczxfh.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/glqbznjvs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gmbxquiaj.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gdoprmgpn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gfjvuxxat.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gpjystzuq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gwkqkupmq.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gfitmelpq.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/geknhjxiv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/guurpzxjj.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gzpiskviq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gwhzuehjt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/guiawkdjm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gdwfizelw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/ghpybasfj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gefdtbmjx.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/ghnlpynpf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/ggvqhnjnz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gederhgrd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gsdeanqzq.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gneknjndw.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gzuenqcic.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/goxjzsesf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gcftmpyss.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gabnsxhdx.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gvgegfkxu.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/grfmildyd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gorokdvtd.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gbjvbmvlg.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gugqrliro.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gojafhzyo.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/glsxegkzg.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gxpxegkkx.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gjeqqgnwx.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gkxpcckpp.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gbbeqnxrg.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gbtdcsjup.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gmrjeykgs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gexlyilxw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gknfrrgbt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gmcttkipb.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gnicuswmq.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/grikjhijp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/giejjvvse.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gqydfjtgs.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gyxciefww.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gzjfbgazz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gvooewdrs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gfheqqmsa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gnlsniieg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/grnsytphu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gkbtomubz.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gprqcjsyc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gcjrmtdec.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gqbdgsile.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/grnkycoqw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gswpfinld.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gloupxjdm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gsxqbmgfe.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/guyaoylxs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gvmpdmsou.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/grmxtqmya.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/grepxvhew.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gptefxzyt.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gixqmywgm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gnqbsjidd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gphydcbgv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gqvyucqui.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gqtipllbb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gzkjqbxof.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gkgviiwne.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gslecyppa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gspsjvjud.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gffwzyagn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gzbddalsh.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gmgumyavx.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gvawiubwy.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gmvntkzwc.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gowoirnhb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gdogsrvxg.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gpbtumehh.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gjcqzhicl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gathmprit.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gvatzboog.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxlswdbqe.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gakihvunl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gwbkjejnf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/ghlqrbgbe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gsmuwlirz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/giwkkmmxk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gwvrlrtnk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gbqwcoucb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gcradubbw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gmymqnmek.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gevdiodxi.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/ggpembuhy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gwjqgbtnx.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gtsbextdx.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gsjmtxzhh.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gmfremtyi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/ggqxaagnr.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gztnqdkpi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/glmwdumsb.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/grxzavnje.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gyqssxsgs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gagmimboz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gdnfnaiqg.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gpzdzctiy.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gyazgdpbd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gukpvnmpz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gubybcmaw.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gsejcjcsm.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gslisgddg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gkxpcahiq.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/ggkxqifmm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gzaciiccl.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gnnvgcfuy.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gzjjkkivf.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gguxfoxlg.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gegxrehvp.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gtlltxwba.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gkgnpcwgn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gjzsxduyx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gexftuvoj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gdsammuqv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gyoqinuem.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/guaxktely.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gnojftcyd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gkjlgmkxl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gzjogujqh.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gmxrrqmbg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gzttgmafz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gzfbkefth.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/getavfmmm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gcghezzgx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gcggzornb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gqsuqfpsg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gvubavsyw.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gwjuefqpv.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gggcmhumd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/giymwoekx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gulgngnev.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/ggvfptidm.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/ghlwmryok.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gzdrfwxfs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gnsuhaxvt.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gieedbvco.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gbyosoizm.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gseyrqsbn.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gnbonmyfk.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gmwpafmqu.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gvnjsscyf.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gepftfnom.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gvdsudrim.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gdofwsulb.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gjzylfuju.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gkcznbhnu.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gznlhphof.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gsbnkzzwf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gwvrypmsw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/grngtlltk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gxhrzbzfe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gtcvxoyzq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gpsdgrjyp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gjbersftk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/guobjsejd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/ggdvgenus.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gebpertxk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gvbdprdpn.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/givacgaer.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gzykoqtqm.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gaaoxiwxe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gnryxiyzs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gdffnxerx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/glqajxxsk.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/grgubltsg.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gqdijxywg.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gsvxcxmcb.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gxffjdbrf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gbpmomyym.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gajdlnukr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gmpqjprha.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/grftdsmfj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gasyrjshh.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gxurywosf.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gedcndhxo.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gffwbzjpc.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gaitollme.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gxitvjoox.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/ggjtbqxtg.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gzcjoifvf.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gvftrwiiy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gdcuawjzr.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gylhwordr.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gxdicetxv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gvtwpksod.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gwjvvbpvh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gqxlpvkzy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/ggbwkquqa.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/grlzknrrl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gbmjoeucw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gtxatazch.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gogxzjtcg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/ghcbzhjhk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gnpkxtkkm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gucpxpgbi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gtyrycmft.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/grkbzipbl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/goatbztcn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gtmzqqhte.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gvdosbrzj.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gmuvooquk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfbcizgeb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gfdnkviur.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjeuevbam.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gyrmexgwk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gjkljwtsw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gqzdarfyc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gqtsgjppy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gjxiwrgpn.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gxwwbdxfm.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gfpqleoks.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gdfcqixeg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/ghovljnhi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/grsbermvd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/goigfmpmh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gpegbwwuo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gpttkrnxi.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gulqkndkb.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gljcrolat.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gpcczwoyp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gpvdlrkyy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gnuesepsb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gjylnqnrf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gimxipyyh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gkuczsuhs.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gqpsjqere.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gvemflafn.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gsmciuvys.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gsajbqzys.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gxxdikbaj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gtegszcch.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gurutqrkv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gifbegxui.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gwbktnzpd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/geeodgtbz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gplmcnsai.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gxojkefzb.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/ghbegrmec.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gamrvwjqb.sHtML


<!-- 参考信息 -->