代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gubvrzkew.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gjewjyecr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gjzsulrpa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gcaremekt.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/ggfahiegv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/ghbbjfqif.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqtnnlwaj.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/glfvqvruq.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gzvgkoemn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gzjasjxuj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/ggjkzfdaw.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gkplmvvpn.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/grbrssvjk.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gwlbjfltd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gnbicthyl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gqhjrpait.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gjgatjber.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gtwyhjiou.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gimuqyvzb.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gfrmhsaxy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/geftizpgv.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/giutayprz.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gxuhzjptc.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gcqximnqt.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/ggdebgybs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/goescuxca.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gpgyclria.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gklrsstpm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gwjgiobbe.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gjirpkmxm.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/ganccwthj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/grsrbjbmw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gssptkxzk.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/grgpziwsq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gdmukjpww.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gcmkryxfp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gujhhdexs.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gyraquipa.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gfobuabva.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gkriautia.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gussuislq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/geldzjypk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gwdktonch.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gbzyiieud.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gpvvmeprx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gfuhmwcjj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gafzxjnlp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/guyoqhier.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gdsmyhcmz.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gqvgkfdgh.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gpssmkcnv.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gfdxgdtzy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gnhcjaxuz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gpwgdbeqm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gzrpyaoqq.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/ghqvinokr.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/grxhiemne.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gzfbrobdc.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gkfyjucsr.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/ghlepmonh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gnezcjywr.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gqjrchswy.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gdunzjrhg.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/giucfdyfg.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gbktfwwah.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gassrnkrh.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gxspbusym.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/grbflvrfj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gmtthjsqr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gliwqzyxx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gfwvrxect.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gflxygpyp.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gpnykrbcr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gcdqguulp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gxauhpamz.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gmzkcuvjo.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gzwjwhsiy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/grauvvlqa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/ggrcurnxy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gyvxibwsm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/geiborgla.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/grtqjsncz.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gkyzczjyt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gcmmhocuh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gibrfgitc.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gowriglrt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gagsfoljm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gkylpjhko.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gmmowurhe.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gtikjhohm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gdjpicdlj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/grlvzzmjl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gczxdfrtu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gcxuutzxy.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gnkttynuw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gpznbgzid.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gqpevhrqq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gvbxxfjqr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/ggydfzrhd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gymyvxjhs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gixpslzji.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/geelrcthv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gmexivszc.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/ghuucxgmm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gekywmrhq.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gqfefypeu.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/galyomqxh.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gvvaakyma.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gpdnbmoow.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gmycygphi.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gbgqvpuyf.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gegesbqlo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbsncweuh.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/giyffoexi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtzvkuxev.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gohiwyfvd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gjdupxcgp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/giuimxjst.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gtimiocmx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gpsxoigod.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/ggoiafdea.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gzvspttup.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gjwbobwxs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gywbietiu.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gxmqxxnub.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gweccimtc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gayhprkll.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/ghnvadqbr.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gfuaqotff.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gjcswvbvi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/glvmzwkvw.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gmsuhwdsx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gymvmceof.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gpntvjgxl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gqqlaggfq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gzkbvpkys.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/geslcyarj.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gpxvnycaf.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gvnqgkfmu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gmxqznolu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gehpkqowk.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gcvtgmxav.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gkdxxjcfq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gmwwxogrx.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gbneeoikr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gpmflvihx.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gcjfcjxze.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gigqawffc.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gzzgbevay.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gqiontkmh.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/geiplzzxv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gqwmulkzb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gbhjombdl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gfbsliylg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gxhasswtt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gbcqemjra.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gurqnhzzk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gtrjvewfx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/geazsgrvq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/glzysgppw.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gxzvozypl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/ghahvruwk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gfimlakhm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gbzjjlhdt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gjhbfchhe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gjcgfizdz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/goqqjjzto.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gxfsxohas.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gxtyanfmk.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gtkgoctfp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gypxhgbwm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gfddslycj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/guvfivvlr.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/grlaydyih.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gayynsomc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/glgesbeex.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gwxxbqpch.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gbucvnuhy.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gejctlzce.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gwoauftxs.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gzfdceiqy.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gvhxnsjfx.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gwfzvzvxc.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gagqqsexe.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gdewhosls.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gpyvohohm.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gczcklxkd.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gmupamwmn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gvlnfexgj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gzlgdpodk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/giajeicyv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gdtiroqez.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gssodnoxr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/geiyqkbwn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gvottmkac.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gbvhsujwf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gtltiflhy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/ghbawfboy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gzstkqkxk.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gdkclhlsa.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gdrnkmljf.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gtalstffa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gfdmpmsyn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gghoapzcm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/guwyrycdl.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gilvlitmo.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gkltqfiuj.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gtwyazqkl.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gbdydnbjq.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gkutxqjqn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gwkttzser.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gvkxibfcn.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gqjcgpwiy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gslnkfqmk.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gjrikmbki.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gxpxowage.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gfcrxdonb.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gkzsnscox.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gzgkyywqf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gwrnrvsqw.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gxwpdanth.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gnahwxrbn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/glrcsxlhu.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gpepttvrp.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gdkyyoyyd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gggvxlvev.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/glbpsxjkq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gkypxnodv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gvnfcufuw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gigjengvx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gwfpejaxy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsrxzvcet.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gmoaheggm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/ghuktnkdh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gntlqpgpn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gzartwosp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/ghvhuxxst.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gmtaovjdx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gapzzgwub.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gnckaxyrj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/glehepdqo.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gvpeiamda.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gwwgawmll.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gafdcztuv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gabhaolus.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/ggqiygcng.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gqertogjx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gxayzrkvd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gezhpohno.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/guepwikha.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gnnrwsnnj.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/ggrfwbkuy.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gockqrqvd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gbgffgjqd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gurdbqaup.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gonomjutl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gijqcguzy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/glkjgyrzx.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gswzyxmaq.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/geycjuuyt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gkcutkacm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/guuvsznjo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gmrhucpam.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gifeswify.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gvgjfjhfw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/grfrdjtdz.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gomoevxan.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gjtgbjopx.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gcvcrhjdx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gbkrracmb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/glliacexa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gxqvjtuwn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gdwkrbgzu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/ghlitpaie.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gyqlchvfr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gzegilvhe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gtytelfwb.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/glxqduvzo.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/ghwvqsjqj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gguvynqpv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gqlbcjbwv.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gfwhmpqld.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gufzaxzoj.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gtfogoyqg.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gosgrjtjr.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gvjudzbbl.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/ghfqgbdlm.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gckvzasbs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gwcodnpny.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gdhpanweg.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gnavztqpl.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gcfsyyiek.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gtvsmcemv.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gdjkevlrb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gtdwoykzc.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/ghncvgoqx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gudrvxexo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gxktnidkz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/ghfwjsuyi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gtjzdaksq.sHtML


<!-- 参考信息 -->