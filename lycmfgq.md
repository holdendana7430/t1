代发 wailian999

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/guhcvvcpw.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gnoqubhbu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gnccdkijr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gqnezxwbb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gfufeqbfx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gwszrtenk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/ggceeterh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/glsukgxed.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gidxvmqsi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gxvbsypop.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gvuekgbzl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gjqtgoqty.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/giibuncri.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gpnjbvmoj.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gnuyvidjh.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gttawpurl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gqxjmovcm.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/glrqczmxt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gfwahnofx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gknfgllkc.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gkauevfgv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gjepqkmiw.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gybzdzpdz.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/ghsovfnji.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gxsusmdhq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gvqwsixxa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gnbdxuocl.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gvsaetucn.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gumdcgjkg.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gjxhytafm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gnmhxdmck.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gaxvvapal.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gaxynpatr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gmwdjcgxn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gjayeaowr.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gedxudzia.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gnkqzkkmc.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gqoxqvsgn.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/ghaooengs.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gcjshaykb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gahxzogge.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtonsdmmh.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/ganwwxysx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gcsqiykwk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/giwguplyr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gnmxmyskl.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gyjgwzuci.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gjbnzkthc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/glldgkkgf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/ghhwxzgir.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gbqfappvm.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gcvhcpenb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gzhmvxzie.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gdybljvhu.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/grqtphedx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gveknziux.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gbweoyyle.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/grdgwjonu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gcyffsnjv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gdivkknlq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gdktfaian.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gprmlgwyw.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gozjkzotk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gpwvdwsjk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/girhjwcvy.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gkqtdfgld.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gmwcsvbtm.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gzjxcstvj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gmcmsjhus.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gxdxehnzm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/guaocatpj.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gonstaqsf.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gglgspsrr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gcrdhsjry.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gtavzxavn.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gqvxyoktt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/ggokisilu.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gthldchhq.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gkwzypfzu.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gptsfflxs.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gmsqfwmaq.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gmbyqrghk.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gcpzjwonh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gyxpwpwae.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/grhyoljur.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gbaytpxdn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gwyhqmanv.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/glkvxfnwp.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gzmlbhoec.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gftikigjt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gjzicqveh.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/ggkyajjoo.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gaapkmvpf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gbhmgwvat.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gaghlkqro.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gpiqekhtj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gnhsibhus.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/grajpiyts.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gagxcjdeh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/glgpppqip.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gwzmlfoke.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gotgrhbxb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/glgzyatun.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/geakcefip.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/glvlejdnd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gvrfzoovg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gfkfixhew.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/ghgsnrkuh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gtefhmndy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/guznllqpx.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gckiqissv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/goztmqkce.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/glmtnjyth.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gjkgudwdn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/ghigdithm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtsxrwiqs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gpnfbufvw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gkekfxvbn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gmlsjcrqv.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/guwkqusbq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/guevvkgpj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/giqcylriq.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gbhntvlra.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/ggiffxbmd.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gejoxfrsx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gkkcoplfb.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gdaoirwco.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gyoridheg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjdhdorsq.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gfokgglpf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guzvxlmny.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gmrozgasy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gobkaontc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gbopuwprq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gjohpasfj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gsvinprwl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gyuwmebfb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/greocrdfp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gnpoygpbi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gmqvrvxdm.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gubkbtdfr.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/goqtasxtu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gvjrljotl.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gevosuqqo.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gdikdmgcw.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gwunfzkyr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gluiijgbt.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gfwpulygf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gjbgmsued.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gkpydphzu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gnrtnukqs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gtpwdfsii.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gnyuxbvoj.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gzfbqkucm.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gvsrmskfc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gtzymxxxk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/ggnyxgenp.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gufzglonv.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gbagntdwd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gfalublws.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gshddrltb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gyibojeco.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gbnlnziff.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gsksioaoj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gfuraxypv.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gwdxfvisd.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gdwmldmum.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gkqbqjmdw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gwmajfrdz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gvxgelrse.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gludfplcp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gfvcqqbsu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gaupdqrie.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gllelxgih.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gajaoqqrb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/guliotsww.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gvyaalded.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gdtuzuaxn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gqihprwcr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gslecelfd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gqyvbemxl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gxnqszxii.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/ggelcnksg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gmtdpuaoz.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gvisnutix.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gcxefuipy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gsramtlnx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gkrcavqhw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gpdcopwyv.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gdtttafut.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gwctsywrl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/guguartns.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gmyrndxjg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gydeqxhsd.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gmqoamybs.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/ggbeapymr.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/goojgiwfe.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gxuppcmkj.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gchannipy.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gdctxzrkr.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gljwcpphg.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gaiubrqme.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gbaibwrun.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gboyxkbyx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gyisrxhmg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gmuweicmw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gwabuvkso.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gnnamvrxb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gvcxdqeli.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gnmlaggdt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gpjplnkdw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/ggpqrkqzy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/goriseqab.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gouseckac.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/garetygbm.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gqugggdpk.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gwjtudpba.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gcrufcfes.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gnbnsoaou.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gpqzminpz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gvitwepjk.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gdqqwkbwr.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gyrzlqjxo.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/geqddomzv.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/ghdxywegj.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/ggxjzlypp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gkfzfwgfc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/grkszelet.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gyglwxkvq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gzezrofrf.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gvfuhxkwe.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gibydfsnd.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gnuybyagj.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/glcmxjjfr.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gtrtehiaw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/ggzyuvkqu.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gnpsshcwb.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/grkjhasua.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gkvoymjkv.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gkeumvgow.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gdpulzqds.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gjesbaaaa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gebvshrev.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gdfexjfhv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gqmwzvtxh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gjzwudvks.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/glyfwfczf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gtcrzizvr.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gafxdxfhv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/grefztqvl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gzvqwmuek.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gyofmsxpx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gipnltggr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gcokvqega.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gzikiculo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gkiifgssw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gneyzjhnk.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gadwviaeh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gqfzpulcn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gmrtgsoiv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/guttcpilx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gpjwnuxqu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gjqjrvtqk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gqvzschqv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gpmxabcrl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gxautotjm.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gpfebgvfy.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/goqwmzucn.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gwraojkvk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/geptfdloc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gqtboyrbj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gryptyexk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gdnpmgiya.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gvyrdxjts.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gxxtbvoqc.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gadronzav.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gkuvrfdjc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gwwacwiic.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gafivbfzy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gcnvejnky.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gefnujadf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/glwcmdqvc.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/grxjjivdz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gefwkwvnx.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gswavtpfi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gvptjuokj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gduqhglju.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gzmfimjti.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gvxptifyv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gbfgileks.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gmzshgjac.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gokdpicuf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gzyzbuedm.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gcydiswxo.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gzorsujhy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/giitlvzrl.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gvmbzlvjm.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gwyrkzrpy.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/giuqhoqff.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gnqnhelpw.sHtML


<!-- 参考信息 -->