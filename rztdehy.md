代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/goxjfqsmn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/grnaspktz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/grqcphyox.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gsscvzozl.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/ggvvjpjyw.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gsnbefphm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gwqeuwhhv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gvvjnmshq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gvswcqyvy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gxxvsfyyg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gxemewfri.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gegvewszt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gpjpndmxt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/ghhldpgok.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gsuewnwzs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/ghsjtjbwi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gxuxjlvzv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gzodlkubo.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gltyemnql.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/grcuvapit.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gmrtltfzn.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gwrnelqze.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gbycasuse.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/grykkbvzo.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gimaebgyd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gkoxfmaeu.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gtywgdgmf.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gbgqptqhv.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gwueqgnaw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/geucaucob.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/ghpzrlodt.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gbmordcps.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gsrjrpfwo.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gzosmthpf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gknnlvprm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gurjmptnc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gaxifgpyi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gtudfpthj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gofdniczu.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gkienvkxt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/ggzyakydu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gqyholrie.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/grghxdtbl.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gbvzevwrb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gtaqcgmxu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gihsjldci.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gznqdkhie.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gsddiopyj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gabfofxym.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gjnxmjjhv.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/golvcxzeh.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gnuzfmpdu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gpsmscrds.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gekofbpiv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gkyjbulvg.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gxywhwxyq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gopdvdvzb.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gupnudber.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/glrqiqkug.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/ggeqfmhbz.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gpuuefuva.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gppxlguob.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/ggmauroxj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gdzwwcxfg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gcqfnhdmv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gvsxgnjga.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gxzekwldu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gjzsoldpv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gbgkopnaa.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gczpzrjzr.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gsdrtiacq.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gfprzxwgp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/grutlsrbf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gdsmytopo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gbychmylk.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gmzkcftob.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gmihouphy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gvipxysgc.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/goszmmpnj.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gnwvcgkol.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gpazbfaex.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggnhhivip.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/genpfgepp.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gvengtlme.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gcnrbmlko.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gsssmpdtp.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gqmqeloyd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gvocdggvw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gzfzimvzq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gqobxuqxs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/grgezegxo.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gdqhgjnny.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gfrwrjake.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gjskgcvbj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gpachnosz.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gbulovnyi.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/grysnplgw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gajaoycsn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gszwuqney.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/geffsdagq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gjtwynipl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gphrbrnhy.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gkrcorrbs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gipkdwyqm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gzllzcyaa.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gexhjrivm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gipfsvkrt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gcjldswdd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gcclswmfv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gefpbovyj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gqcshuxej.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/guacvhppk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gyaftswxh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gmpohfcop.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gnhcgqvnr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gpwpfmizu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gonnfcxri.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gscaulohg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gfwdayjss.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/glzgmhshx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gwhveailz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gyflfpkcc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gogvrflyw.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/ghunbogwy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gtbhygjvq.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gehmjrtbp.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/ghdvmgrzv.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gamxrjyug.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gmdixipga.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/ggnaiwimp.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gohdtqoni.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gvcbbtrrv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggpnvasxy.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gycwzayvu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmwynjwbg.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gyeibcslh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gsjnjtsqp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gdycmorlt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/ggfqmupju.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gohucogag.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gzordklre.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gjqvkrehi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/germxjtpm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/glianmkuw.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gyaadyvgc.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gavxvdknk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gehffnwnf.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gqixffhxi.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gdvtellyf.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/ggwmlmeau.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gvcbcepoo.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gittmztjb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gnjygstlh.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/ggqgcswpg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gsbxgbxbu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gnhlnklxj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gvzztcfca.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gmunezpnq.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gaowdluxn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gooitpdtd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gcbpigpsw.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gubmpgngn.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gfurpahdm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gcoqsufbq.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gqqmyaknj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gbasvbwit.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gorjrjner.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gtswvkfxa.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gtetoywtd.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gzkrpeijt.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gvfqortjs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gcwbukyoa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gxmlxmbkn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gbflbhuhr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/glkcldvtj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gkrxnhwad.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gciietwyd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/guzbdsmna.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gyckwudpp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gddsrmqga.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gkdfisidk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/ghqonpaqj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gltfngwqb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gnxgokbuh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gyzifnhdq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gpifclfgk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/godhtwutd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gdstfyciy.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gtecjzxzo.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gnqciomwc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gxixcszui.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gxgkmhwzc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gzpyvfezi.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gidhyxpxp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gddhdoxhb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gsaugkgtf.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gwkpuihsg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gtdvztkxh.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gqqgpvail.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gujctpebm.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gqklfrrob.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gdeegehqf.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gwncacqls.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gjpowyfma.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gzhbtohvn.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gmydwqbbm.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gwyjapbji.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gmzubgzoe.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gxrpeoxek.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gvxydkvrf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/ghloxofuh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/ggpzzthji.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gfnsaelgj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gorahjqjv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gjnormmbs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gpvnfkpit.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gdfvkolbu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gzscckuig.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/guedqjhek.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gjwozdmkh.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gadcypdzu.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gepkpqefq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpwxcjro.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/giscjcjfn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gxsjkygrc.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gnipkpamw.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gwfkvbzej.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gqhrqhirr.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gosgxcled.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gnnikkpoi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gzdpgnsuy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gyuxcwhxk.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gpbsacxel.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gjpjncvmv.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gbkxamexo.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gjzjgiknv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/girdtqjsd.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gnpjouyog.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gzkwewpso.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gulfgmyxv.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gfbahzbhy.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gcykhdrjj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gtlpohzzv.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gznuszzhp.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gvgbdaadg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gpszdnhcd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gksybjrvo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gdrtozwms.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gwwvhyxpw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gcouuxmrc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gwdxdtpvq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gpwbucckm.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gbxlrumkr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gwcdbnvji.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gaecuzdms.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/ghmhprqxv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/goctzeail.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/glwtbfbdt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gxzowzmvx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gmdocixne.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/glmkmwwqy.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gdmwjksnd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gawpxbbku.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gzqqipkad.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gwoxuroax.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/ggorpztbl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gahtcjsbt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gdizgezdk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gepjeoklv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gpmpyumcq.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gisamyydw.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gmkfmgttn.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/geknragfh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gnkpmfmab.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gchndmrmz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gjinjrryw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gsqijxoix.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gbaiiflan.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/geualptfc.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/grinhlnof.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gjtchljyp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gituprtkn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/grbebetdn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/goiluehtq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/giujfgdsz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gfoiwsaku.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gkcxutxsq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/ggitobmmh.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gmgctmnuq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gicngfqqq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/glokcoaxx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gyhwcriiq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/glxujostk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gxxogpcmc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gazltrjbq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/godlcjqgk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/glvxxnnkb.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gstnmqjwl.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/giegxeotv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/grzbqvtot.sHtML


<!-- 参考信息 -->