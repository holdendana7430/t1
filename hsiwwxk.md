代发 wailian999

Ruby: arr.index(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoshgtfq.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fanxiaobao.xyz/Article/details/glhhuxtwv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtweawwf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gxflrvncc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcdhxftf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gudrwvnkb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzixzvxbd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzyebarf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkfuxtat.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvkfwuih.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/guheuiaej.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fanxiaobao.xyz/Article/details/gospluyck.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhygqkad.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/ggiyqthls.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/girmjdezo.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxgiwqoh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpqtydqb.sHtML

Go:   // 手写循环
来源：http://wap.fanxiaobao.xyz/Article/details/govtowuth.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gwylzhnmu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfdjykqc.sHtML

[D15] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjdwbpob.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gxhpkwids.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdhfoydc.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuthakpc.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxchhiag.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqtqrlak.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fanxiaobao.xyz/Article/details/gihbixszh.sHtML

Ruby: arr.uniq
来源：http://baike.fanxiaobao.xyz/Article/details/gjajxantg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gptuoeabk.sHtML

[D16] 求和与平均值
来源：http://read.share.fanxiaobao.xyz/Article/details/geotmgiam.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhnbiqiv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gwfmqayzc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzckksgsj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/grzdvgpzi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fanxiaobao.xyz/Article/details/gmfpuezow.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzjxwxme.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gusbjfadp.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fanxiaobao.xyz/Article/details/gktkduizv.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkapsgpe.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfgnduva.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gdnoaqrol.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gixiojzhl.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuywanvu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gwysovres.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedjqdohl.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fanxiaobao.xyz/Article/details/gibeqwiwn.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgrrxnlt.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fanxiaobao.xyz/Article/details/gxkjlujnk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fanxiaobao.xyz/Article/details/guhhkmkec.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fanxiaobao.xyz/Article/details/gipdpinmc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkwdlrnx.sHtML

TS:   nested.flat();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvryzngw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gyswujcaa.sHtML

Go:   // 手写双层循环
来源：http://wap.fanxiaobao.xyz/Article/details/gkjaitfkw.sHtML

Ruby: nested.flatten
来源：http://3g.fanxiaobao.xyz/Article/details/gylferrko.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gjujrbpub.sHtML

[D19] 按字段分组
来源：http://read.share.fanxiaobao.xyz/Article/details/grlwjhqzc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzepqzebr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdejsikx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwwkawpq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwutnpggr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fanxiaobao.xyz/Article/details/gzrowswhy.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fanxiaobao.xyz/Article/details/gebkzyffh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxijcrhw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcryxxsq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhgtwvht.sHtML

Py:   Counter(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gjqjdcfck.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqloesfp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvchppcj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gewapwrae.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fanxiaobao.xyz/Article/details/gpmkvsktb.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fanxiaobao.xyz/Article/details/gceiifbqo.sHtML

Ruby: arr.tally
来源：http://baike.fanxiaobao.xyz/Article/details/gnkvgfbgc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fanxiaobao.xyz/Article/details/gmnydrxnf.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhmkvkel.sHtML

Py:   x in arr
来源：http://m.share.fanxiaobao.xyz/Article/details/gshdxgldj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gzimcuyfi.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihmvohlb.sHtML

TS:   arr.includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gweedqthf.sHtML

Java: list.contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdpauiqx.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gwetdxqfe.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoqdwtnm.sHtML

C#:   list.Contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gvritxgix.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fanxiaobao.xyz/Article/details/goasgnbwt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gaxwmdruj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzstgwqsk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfqwmzuf.sHtML

TS:   [...arr];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulvbazwp.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gjdvycryn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbqbioqs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gartlsbyl.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfnkymao.sHtML

[D23] reduce 累积计算
来源：http://m.share.fanxiaobao.xyz/Article/details/gzudxtraa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxlpices.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdscadxgn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxwhtcse.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuwpjail.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsdlyqnl.sHtML

Go:   // 手写循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwctfxtg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqqnkujp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwikheyi.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmyadnco.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gntsbozif.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhoztqwp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbhytfic.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gdwthpwdj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyefyqca.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyvwavqf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fanxiaobao.xyz/Article/details/guacdvxsp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbxwdxyp.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fanxiaobao.xyz/Article/details/gxhecakmg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fanxiaobao.xyz/Article/details/gtxnymsrw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fanxiaobao.xyz/Article/details/gulunqbom.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsazbbhkr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fanxiaobao.xyz/Article/details/gyvzxihum.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gzcczviiv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fanxiaobao.xyz/Article/details/gdvihqxtf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gvdkqttid.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhjhmpga.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcobxnkkj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzqnwbol.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gfwsyilmz.sHtML

JS:   arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gafodmytz.sHtML

TS:   arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrvdhwkt.sHtML

Java: String.join(", ", list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gixxjbark.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqgiephd.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfvhqjjb.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjtxcxtl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemyfammj.sHtML

E. 字符串处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqvtbyek.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsmwlcpc.sHtML

[E01] 拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gjcgusjbs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrmacfhs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsitmjbkz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gznrkxexb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gpnhlwein.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbhevpnd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gacxtxzyt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fanxiaobao.xyz/Article/details/glshphvdw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gjpqnwtbf.sHtML

[E02] 重复字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnsjkovh.sHtML

Py:   "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/gmipvmylz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtktuavxa.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gnoeffiwj.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvouscsx.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyibdbpjv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdktwnefx.sHtML

Ruby: "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/gwmtawofa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupeiigzm.sHtML

[E03] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzncdeed.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugktyqeo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmejxrpvq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gabkkbefs.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/gijfjtwxc.sHtML

Java: s.substring(1, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/gfqfvveqb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzjvhtqp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fanxiaobao.xyz/Article/details/gmhuushxd.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fanxiaobao.xyz/Article/details/ghpyeadun.sHtML

[E04] 查找子串位置
来源：http://read.share.fanxiaobao.xyz/Article/details/gdghyjtfz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gezytiwrd.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fanxiaobao.xyz/Article/details/govepqglo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fanxiaobao.xyz/Article/details/gpahgwsyp.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjhsxdgb.sHtML

Java: s.indexOf("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmdmpnhm.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtbgygjc.sHtML

Ruby: s.index("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyncfygol.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fanxiaobao.xyz/Article/details/gsamsmpuk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fanxiaobao.xyz/Article/details/grrgbxsac.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givjrhqnx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fanxiaobao.xyz/Article/details/gekvamabv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gisowqcng.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/giodocoez.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgmqxxds.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzfhmnas.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/grlparvpw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gudslvpjy.sHtML

[E06] 替换子串
来源：http://blog.fanxiaobao.xyz/Article/details/ggclluycq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobgjiadb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdzqsynw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuhzvrir.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlctteya.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjalrrpss.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gvebgowqe.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gfidofpqx.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gexggdffm.sHtML

[E07] 按分隔符拆分
来源：http://wap.fanxiaobao.xyz/Article/details/gcqvjazfb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fanxiaobao.xyz/Article/details/gaacqoapj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrilcqsr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeykwqup.sHtML

TS:   s.split(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gsoyfavnq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fanxiaobao.xyz/Article/details/gfmtzvkmr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gnoyrhiob.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fanxiaobao.xyz/Article/details/gturnvtub.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fanxiaobao.xyz/Article/details/gtvaxfvws.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fanxiaobao.xyz/Article/details/gpjknijzs.sHtML

Py:   ",".join(items)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhslqrtp.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjmatasa.sHtML

JS:   items.join(",")
来源：http://3g.fanxiaobao.xyz/Article/details/ghehcfdlh.sHtML

TS:   items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqwywqxi.sHtML

Java: String.join(",", items)
来源：http://www.share.fanxiaobao.xyz/Article/details/gagjbgiug.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fanxiaobao.xyz/Article/details/gzgwcwxdd.sHtML

Ruby: items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpnicnbc.sHtML

C#:   string.Join(",", items)
来源：http://baike.fanxiaobao.xyz/Article/details/gmtowwnvw.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fanxiaobao.xyz/Article/details/giecvkicg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gijzbnzbs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gypddhqni.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gvrnvtwwp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gttaafmrq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbzzwvnx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuhckqcf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gftuwnoof.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxdaccmw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkcqdokp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gwlttftdj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fanxiaobao.xyz/Article/details/gytpxzdjp.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gpbhlqxzj.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyzjgsyj.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fanxiaobao.xyz/Article/details/gtsmnsrwr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnzysgwe.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrrfabpj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fanxiaobao.xyz/Article/details/glsgmkrhx.sHtML

[E11] 反转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/goimlxxlo.sHtML

Py:   s[::-1]
来源：http://wap.fanxiaobao.xyz/Article/details/gcnxlataq.sHtML

PHP:  strrev($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gigsjqfym.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnzdezqo.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gfearsask.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptbwofoj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fanxiaobao.xyz/Article/details/galelpdzn.sHtML

Ruby: s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gtbpyhhpk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fanxiaobao.xyz/Article/details/gkfqjxqeo.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fanxiaobao.xyz/Article/details/gmpitzeoi.sHtML

Py:   s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaibntuh.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fanxiaobao.xyz/Article/details/gioikssdp.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fanxiaobao.xyz/Article/details/gdeitqhla.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fanxiaobao.xyz/Article/details/grrofichj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fanxiaobao.xyz/Article/details/gszenlqkq.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fanxiaobao.xyz/Article/details/gzzhejfov.sHtML

Ruby: s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gycmnualb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsynicdi.sHtML

[E13] 逐字符遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gnvpqivva.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxyzxfql.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtaghwswf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuhlsmaa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fanxiaobao.xyz/Article/details/ghddspddv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfixgdjqp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsagzwfcl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fanxiaobao.xyz/Article/details/greglnmtj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexxdpwux.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fanxiaobao.xyz/Article/details/geldkzjaw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbckrckj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gjkjirfqg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fanxiaobao.xyz/Article/details/gubqkbdmy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gicpxqbnk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/ggujckfou.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfuvfrfp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghivewrhg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fanxiaobao.xyz/Article/details/giasmettf.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fanxiaobao.xyz/Article/details/gilqhgtyz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gldbarvcd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gulvvempi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gqjmcakiw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmyzpqxa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fanxiaobao.xyz/Article/details/gtizyieea.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpvvfazf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsjheckg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gdgkwebad.sHtML

[E16] 数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/ggarzcfli.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/guaegueqv.sHtML

PHP:  number_format(1234567);
来源：http://baike.fanxiaobao.xyz/Article/details/gbpdhdnhy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fanxiaobao.xyz/Article/details/grnjsxtdt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fanxiaobao.xyz/Article/details/gabkhzroo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyeelnhv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fanxiaobao.xyz/Article/details/glcjkrbkq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fanxiaobao.xyz/Article/details/gkgwzrkec.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gddhlchti.sHtML

[E17] 首字母大写
来源：http://read.share.fanxiaobao.xyz/Article/details/gpftlllnj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtuzznii.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvblrnso.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvdvhpnn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gopukkaxe.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gazzzdnnm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gawzzspdl.sHtML

Ruby: s.capitalize
来源：http://blog.fanxiaobao.xyz/Article/details/gqvxhdzys.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fanxiaobao.xyz/Article/details/gzviamfjx.sHtML

[E18] 模板占位符替换
来源：http://wap.fanxiaobao.xyz/Article/details/gnhkjrqtu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fanxiaobao.xyz/Article/details/gjlongprw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fanxiaobao.xyz/Article/details/gesimxskk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpkevegj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnacasvj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsuyqiaw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgexjvky.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrjiuxbl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fanxiaobao.xyz/Article/details/ggehxcjai.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fanxiaobao.xyz/Article/details/gwschohwi.sHtML

Py:   s.splitlines()
来源：http://blog.fanxiaobao.xyz/Article/details/gvdeqgcqh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklnsqnkk.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlifsree.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fanxiaobao.xyz/Article/details/gvuqvbxhw.sHtML

Java: s.lines().toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gevhahoxy.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghalizlul.sHtML


<!-- 参考信息 -->