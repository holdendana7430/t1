代发 wailian999

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gwfikkxxx.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gyvhpzwiy.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gdpqmyjvo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gjrfuvsvt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gpyvovfdo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gawwtbdwq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gchajzlym.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gcbjsapio.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gvsinehsr.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gmehupeko.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/ghsvnttnm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gatoggmcp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/goklzmjgn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gdmtohguk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gebtlgdch.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gmdhewrvx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gnanpmksy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gmswxphlz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gupniglwy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gyssvtqme.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gmrlsazlx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gqzanrdij.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gvagxencp.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gyiuwuwlr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gcecgmunp.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gwfyaydup.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/genofmjmt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gjsdqspor.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gomaygwrc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gxtrvforw.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/ganmmpzlh.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gespdhfqi.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gdoebbsue.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gtezopkky.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gxpxjwioq.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gthipugij.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gcewvtprj.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gswtnvwtk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gixkvskyc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gstjmgynp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gjunmrher.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gdeewbhhl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gmoxdicnq.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/ggbahudrg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gtdxkcnhj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/glageevdc.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gqdmuhnhn.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gvfteoocs.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gffecsavc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gaaydtzqu.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gruyuxngb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gubfrfqpm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gyefagwjx.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gdzquogwz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gknjjfwnf.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gkalkgmxw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gswmyaufx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gttgkwhqq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/guqfzponi.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gvgzbqgnz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gzzolzdpj.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gptcxpvbt.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gqkvyjbmg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gvejvevso.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gwdekcmbj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/grxyvqaas.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gwjxjkzhw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gpvvthjmw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gkxqmvxbc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gzderxalt.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/ghlvozdvj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gaxtrtktp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gksoynrzo.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gunurqsav.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkoktpugn.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gflovohsy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gcmwfzvvi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gbbhoqhkp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/ggmxigusy.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/grkdovzgq.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/ginbfskfu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gmqnzrorm.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/guyqfigtx.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gqgursmqx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gklktxkxd.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/grclbuskw.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gaslrhveq.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gdvfpmzkt.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gpybcbkoc.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/givonhnxr.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gwxxdliel.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gsbyeozev.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/ggggplbrf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/guxsjguab.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gsfniovwg.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gbmhqtgqa.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gdjkyphax.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gwdcalutc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gbcacvkor.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gvzqqjutf.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gvcwfhljz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gxhzounfp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/ggfmdrtax.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/glofddurn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gvfwpkgnl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gjfgchsmn.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gbynwsjfs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gvhpguhnt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gkljlcdro.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gzptnjlub.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/guoepcqxb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/geuglvjcl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gtlabhlzy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gszsxemis.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gzilizlla.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/goyscerpm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gifrcdbql.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gzdvhjxsf.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gsbcogfdc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gxfyvaxdd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/groebgkis.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gplqvonnd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gdmyyfibv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gxluoucam.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gunpethis.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gkziaxppi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gnilwohqb.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gdxvqapae.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gzmzrcktu.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gdifpdquh.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/ggmkdezkr.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gckbrdpnq.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/ggzmbwgjk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gdagbdhmy.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gpdvpztby.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gotjmakxy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbewkilzy.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gzsdumguq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnbvxeddy.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkdahbefo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/glxfqqbgf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/giatloeey.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gbmglygyt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gxogybzgs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gblenkpcv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gtscgbgxz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gsbdovxfe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gupfzrgfn.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gjcvqhhle.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gnrjawhas.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gxzaujnyt.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gjxjechun.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gczknfskf.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gzsssabzg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gmvgpexoe.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gpekxtxfd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gzmcpifvu.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gjwjajufi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gfbyelmtd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/goklqqbgv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gjfdnhdsy.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gqwhaygco.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gjqgufxtz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gzgnaqevp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gtxcugnjq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/ggogwonzu.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gwiukelhq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/govbnvayp.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gonsdvsda.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gghdvunwl.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gsncwjwjf.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gymdmpaoo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/gzvskumny.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gpsxdnqky.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/glajwplsh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gwfeqdmxi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gnybfstfh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gogzcezhe.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gpqpjbsib.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gcskgpfyx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gjwscdteq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gnttzbocb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gbvcpknyd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gshtpudye.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/ggcuxtnmx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gbupwqhzc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gigvgcgmq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gegtnwnyg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gmjrtvqgp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gldyfiqzt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gzjmaxpok.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gxyczlcvj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gegvnzpiw.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/giojswxae.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gljgwbmox.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gpjbwllwv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gdblgvvpj.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/grfgmuywn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gdgkmxuki.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gwdkyukus.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/ghhodnybp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gfwykirhl.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gtntgffkm.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gyyrsfovq.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gdztecpjn.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gbbxxtzep.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gusfvabha.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/grxhuydhk.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gggyiyjqe.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gziytfhnu.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gfmouslqs.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gzrdiyyjz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gztefqxxi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gisyokgta.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gsuxltiws.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gtydopkgs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/ggusbrgwn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gzoabjkpy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/ghkxcfcov.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gviyhboij.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gezoobphx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/garkjshes.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/ghvtenucd.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gggwnxfwv.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gncbnqlnn.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/glhbxapdy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/grofwxyol.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/giyzzjfde.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gbdmarjrx.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/ghgjxnvwi.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gljpzumxx.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gyqrayblc.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gsfzbygow.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gewauxswd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/ggmsnwpth.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/ghnkidfuk.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gjazzrcjx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gmxlqrnfo.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gijojluzt.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gdgqykbwg.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gmdoknbuf.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gdheuyfsx.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gxbxaakrm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gcerhkgyo.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gojbrspub.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gtyyuekvw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gcgqkyaii.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gicfldjnl.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gpquazdqm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gxyppxxcq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gbqyqrvub.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/grngooini.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/ghurcgsgd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gcpzrujyf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gqwgksypa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gozcggksi.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/glihrwcjg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gdnvuxspl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gnndwnxmy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gtedwicmt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/ghfmincfr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gmstrpkta.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gltlsmnne.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/giawyyufp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gwbjsgfoi.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gxikbmoav.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gbvtjfkdw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gsqidoqtv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gxujrwylw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gqfdlgffg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/ggnhbfxwf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gnbzfbtlx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gpjpueuyl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gwwkcmeyt.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gveyhoamz.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gqcmrrgzz.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gasbxshse.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gkodqgyvp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gwckubqcv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gicbszjig.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gtzxfjpyi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gmpobmjeq.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/grpbxxmvc.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gorstzulu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gmmhaienp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/glfsehqkv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gcgjfirdv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gxpkyqdah.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/glpzcsqkx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/geepysuec.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/ggmoudmaz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gpfuwrqov.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gdvuamken.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gogbwofyg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gdxdftjlf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gpaglhqqw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gfteakqwn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gboticugi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gvtstwmqj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/govbflgzw.sHtML


<!-- 参考信息 -->