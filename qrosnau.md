代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gvdzofong.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gibuzdxie.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gcohdncoa.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/glgnwfwof.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gjrrcwsjm.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gemoxitjz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/ggmkzhalm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gucrakjsw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/guajlrydn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gsffnpqhl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gdzcaggwp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/ghsrpzrzh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/glnkmqzyg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gdvprjauw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gmhldrycu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gpfssjtqk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/guztixdfs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gaditgnid.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gulijagiz.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/guhhfzjfl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gkzqcsklo.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/ghlfxowqk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gdpiqwbcb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gzqszmdeh.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gmiqhonsw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gxdrwtxng.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gpltlwdbg.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gqsjpniuy.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gxieakrlb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/grwdieqin.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gzdoicjrp.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gbjgaibjs.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gzlyibbyv.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gpcdrkgpj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gqcsadrmg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/grhrjuflu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gifaymykq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/ghubhzlyy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gsycadncq.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gntpuxopm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gfonkzpbf.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/grtrlxmbi.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gulebtjqy.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/grjhlrwah.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gctvlslks.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gwrlpaidb.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gsdorgtej.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/godhpdwns.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbfqrkchx.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/grsnkmmxc.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gkgindqxz.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gkfdwwyle.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/godyjdjmp.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gadjdsdzv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gcubhslqg.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/goshchgxz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gcbmitnea.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gdlyywqbm.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/guswtblvv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gkgellcpk.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gnqebinct.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gxctfkbyi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gglnwdzhj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gyrievsvz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/guabobamx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/geupdheym.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gapufothl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gjacprbxv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gzwxmvlog.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gzlcvtgtw.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gxbflbrec.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/ghxwhmppf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gluqrckit.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gofqciboq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gxzldzdei.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/ghhdhsblq.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gtlzoretj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gipnlddud.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gtirteoku.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gfgvgllpa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/ghmjvhyhl.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gwbcweooc.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gngzlngpz.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/ggocbbyyx.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/grznpbovn.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gxugirwfe.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gwhzrllex.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gqymznmhz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gexzhytom.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/ghigcriop.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gbabevmwo.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gtrclewah.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gbzcrpeal.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/grnoiarmn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gfsrnkojw.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gtnopafsh.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/guvsgqdsn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gjmxpztwg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/giwcoegod.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gfuudwwfb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gtpocaray.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gfhndcdzy.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gmwxhrzyt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gryzhisdi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gswbhfcvt.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gjamhtonf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gesivomfi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gtxknvcst.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gvpdnebno.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/glxhkuega.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gcpobygtz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gdbpqubyh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/girlukegv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gvuegwpvt.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gjdwajevl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gujwgulqy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/guojtpjbs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/glbkhchxd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gncmtnafk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gytbscsfs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/glqfpphsv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gdgvvpcwo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gzcxgzqxk.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/ggkvyevub.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/grbilioye.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gdpettoev.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gtycriusu.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gdnmovosa.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gvocimafo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gryhdegjf.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/geuuidsmj.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gcxkltijc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grybdriqh.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gidnpdbbx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfhqcwsxw.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gkuxppeej.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gpsnvlymu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/ggdrxrzhf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/ghvjzgvfo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gckrkxsgt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/ggmjjlkxv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gemcxjqfr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gilpywgtl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gtkdduhsr.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/ghxiiiqwd.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gygjfxcss.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gbgudklcz.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gpwbtjmph.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghnammrfh.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gjmtazrzf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gvtxqmddq.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/grewcivqi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gxcgbspiu.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gdlpgbnqe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/glwemezth.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gsmsoyuwg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/genijjamt.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gergpubxc.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gditdzjon.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/ghajxmhya.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gkwfxgjnp.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gjiskeqxr.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gnzbrervq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gjsoimemk.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gtpgudfmp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gtdmboxuz.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gllnddllf.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gsuvvyepj.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gipxriwtb.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gbfbzdcsr.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gqlimacfy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gauxjbxmk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gdknfrxqp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gvqlordgx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gkltwbsrz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gzrwlomtj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/goilocoah.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gufupcurj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gvihklutr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gqvlvwzbs.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gqpoaegem.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gtxzbqini.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gavrlzboe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gbhyakwir.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gmjwinmee.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gniglrhtc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gghcsundu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/glmeroyfu.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ghmlehqpb.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gtlbvvmtd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/giqnuqmif.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/guqkzsnuy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/ggwqvvbwc.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/ggyvheasf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gfjamlevy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gkzvgjolb.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gikolcuto.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gcjxmvgpf.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/ggwoersgl.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gdckvwzue.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gdxmnxjwu.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gvroiptib.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gnyxavbrg.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gqwfbgiap.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gislvsfaw.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/giqthlsyd.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gzqfskkuf.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gyxopvuxq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gjitgredf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gdsyhqxgh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gluzovmgo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/grtcvilbm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gibccedoi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gyhqfvbxe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gvmkvvtma.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/grikprelo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/guhgkpveo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/grzfucuim.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/grutrmoll.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/glfskvmys.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gkmhnzsep.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gfnzxosev.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/ghzoxvmjs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gqftwjrqn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/glhecbenp.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/ggvwdcypw.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gkdyaqupd.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gzdkntwym.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gqhimntkn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gtntdrkga.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/glfucxrvy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gltixmlxz.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gblzbsidq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gkkrqvydh.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gznpnpduh.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gdtwrursj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gpkteblfy.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gpmfftqgy.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gpdielujl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gvxkweyal.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/ggijfnnej.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/grctfdlgp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gjcltjlne.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gtwpnugiu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gpdnjozqe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gykwrtnts.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gkwzgilzm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gnmtdhenl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gkxfvxzli.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gpidusxny.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/goxjpfrkk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gmhlerwwu.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/godpgrlaz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gwpwhtjob.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gtnxspktt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gtajbghbx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gihmgibmt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gfwerdiky.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gyhhkikdo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gqswtpyyc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gtqkgzbjf.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gtrcuumbe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gahwbcbzr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gjezdoirg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gaoabygub.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gbhmncuqf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gcieatojb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gfypjdxps.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gzocxwfoa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gdnpsaemr.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gqdotqwvt.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gycenqpuq.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/giizypedp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gvoouwpzf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gkaovofnx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gkswinawa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gkhvcanxs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/grdibunjy.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gnhqwvvts.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gasajvhmm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gusbqwrzo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gdsnfidhr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/ghebsbnyc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnwdteptr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/ghqknnbyg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gqrpixiri.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gnckvdprr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/ghrnnkzwk.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gfmhdpgbh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gdohcwvnf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gyxhpucqn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gtradmvrr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gytbudlfv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gzufoanbo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gpldrgwwh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gxvszdcni.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gsvfvugow.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/geoezseqn.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gzrzjdjga.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gcrgeoloy.sHtML


<!-- 参考信息 -->