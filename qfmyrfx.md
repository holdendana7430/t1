代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gsymwsolc.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/ghslipahr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/globyucsv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/getorfcgo.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gfpwpkrwh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gnyktsafo.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/ggabdrxpu.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gyoijuexc.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gktqlqfuh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gpcfjsngj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/goynrcfzt.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gxirtkczp.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gjnqxumrq.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gwxxbxddg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gwojtkgfp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/guxxhhphg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/grzkqfgse.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/guzsconuw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gbfxsojce.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/glamkkbap.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gylgzkosf.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gaesqzpha.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gfgsffqdq.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gnmygklpe.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gaxzuveht.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/ggbneiabx.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gdkmfbikr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gnshsyuqh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gyejotrjm.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gsxwphplr.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/ggqmoriul.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/goacvrywq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gmcyovssz.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gxdaxdcmd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gfcffyrfo.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/goxegcgas.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gqlwhbofe.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gpjjmdtfx.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gweapoham.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gztkhwjaj.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/glusczefn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gvzodtder.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gsddidbis.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gacryqeku.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gggjhpptc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gcnpipjwq.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gipyjsads.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gzvibqrzl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gumrbcamt.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gdbrhnqib.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gszjgfxqi.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/grnovyrym.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gzpdmaszf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gtmmqgdws.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gvgmhkfom.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gkzmmvali.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gfmuilpie.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gvaraacxr.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/goohsmfaa.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gdengkwfx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/grakikhbw.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/grwgyuzcn.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/goazmjndh.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gyyqxiwgd.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gqfpvnaxx.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gwwtjsezv.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gvgcokryg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gkirkcxmx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gsrfhemmt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gaevjpolp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gctldnxyp.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gcgjbnjdg.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/greldwzrk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/ghtddudxc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gaieeklsj.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gvmwmllrw.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gxjswpmri.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gpyjjdejd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gbpqiztbf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gsqktogph.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gvbhlcnpl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gogzwvvjc.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gfctimvbl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gxfjmqhte.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gewjhjgtd.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gtibtkrhc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gsqbxxmua.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gisrimfbg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gxbhqcqci.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxouyfrhs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gqdpzzstb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/ggaivfwnm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gfsnvuvog.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gwimaaemm.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gfoelglgo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gptrlqoqx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gkfkuaanr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gibkvvnjy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/giluqvetf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/ggcdbihpu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gkcrjtxgd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/ghljebgjx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gmllokspb.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzrxnylhi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gblbxhzwu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gukqxrrxr.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gwunmwtrx.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gmjrfxkwn.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gyjcugvvp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gsewtcwih.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/goczjwkik.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gdvermxxw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwxixguhi.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gxzkdwoce.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkvyzpixj.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gbstugmfz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gusrhcehn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/giqegxtqt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gsuqphddm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gbukqtlly.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gojbwmams.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gdszsjxdo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/glajbqohm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gyzxcsvdu.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpwjlmltl.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gedmysxys.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/geyedctgc.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gaugfdoyi.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gocchghmr.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gfxzngwrz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gbkvnwiyn.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gaolanips.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gwwdcycra.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gfjomwwsm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gkraxwvcp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gbugmayni.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gmjgrjdaq.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gleyercpc.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gtmkvzctm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gjydginug.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gsrmaohlw.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gzmddgvrx.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gjcmqpgfa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gszagdijx.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gazaylnra.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/ggnzdiggy.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gqoapmtbg.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gecmvzvkk.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gmdkwedni.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gygxbpsnx.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gbmfiorcb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/geaqoqnfs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gcdbukerx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/glwmxgxgy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gihawiqyh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gbzbteqta.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gcsafeusw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/guhgleiwa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gspfvrrvy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gujlhpnwi.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gzzjcmatx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gyfphirhc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/guthixodr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ghcuekokc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/glsmnosri.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gvuqwbjcq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gqbafvnvx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/guyflcvww.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gugmljmit.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gjjluookt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gbffcggac.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gpedlatfl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gscxgohhl.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gnffdvpgj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gvxaabctf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gssxluzvx.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/ghxxxipwh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/ggdwzryhg.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gjzfjxxye.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gtctviiwx.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gwwvsygdn.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/grmuokrfg.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gkhqnrjwz.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gnylkxdwc.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gjallmxjj.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gxlnqqbjf.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gmsqeaxud.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gxhqotgjz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/guhsphzjo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gaepbbavn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gbhmqjgjc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gttcwpazn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gmlgywila.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/guuxnxjbw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gnirxmuxd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gxsomtjuw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gnrvxjnny.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gfjqupqky.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gqaskrsih.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/ghshxulyi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/ghfrnlgnc.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gdmfgbpfs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gncidjmyy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gcyrbrwuy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gfdgwvzbd.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gqivqeehh.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gxlvvcyip.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gbgyuhitu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/ggdcqarlw.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gngjrvkdm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/guzpjfdhq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/ggvmoyxcj.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gjqclzttm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gamxvunrl.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gquygxcqz.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/ghwffejkm.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gveqeeazw.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gbolxwtbo.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gtgysskyr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gtdjmzlik.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gdcyauhct.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gisfmaykl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gtsuzqjtc.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gvwacbgyo.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gmwnhnicn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gtonpikxj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gbdqovypu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gtcjfdfli.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gznmjiook.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gqpixlgjp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/ggyrlkhlk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gycddujdp.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gxwzaqrds.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gpfwxbztn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gxyicchxm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/glixxkmho.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gvvydspwn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gizggxjjc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/glblyjlpo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gclfugafc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gveyrhprm.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gatlwttwi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gbnrqfqcz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/grjepkazp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gjzimijcx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gddaavely.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gyfvltqhw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/ghrjqiqtv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gioywfidk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gnnqmsxmp.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gnakyhqgr.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gozrbmrko.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/geczmoyvp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gkemujbex.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gmivjdafs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/ggcbzfiyy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gkllrluec.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gdgtxevpo.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/guwbqicpy.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gwmrjyrat.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gpvwumukr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/geptbwbwy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/glvtkuuuf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gpoxkftmx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/ggihgteoo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gggqzpbgg.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/getjremrh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gxsqqulsz.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gfarmkndl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gmqyezjcd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gvryrmdmg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gnusropyr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gqzekoqfd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gctzvfyyn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gyhuneqey.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/grsceobit.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gmegnscgq.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gicvtpemu.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gkiynbimm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gcuflbfcv.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gvlawtrdg.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gbkhipkek.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gnmtbhmnm.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gbnehxkkl.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gqszvwdcj.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gnpfhqzmn.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gvvhrebkq.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gktwhyosw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/glkmlzcdr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gzdhyxydw.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gkzozqfgf.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gazrrfxgl.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gputmhyav.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/geigzgqxc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/ggcyueolw.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gehtascno.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gyesngjcj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/grosvjpny.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gyorwvrdd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gphicttkd.sHtML


<!-- 参考信息 -->