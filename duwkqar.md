代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gwqroarxz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gadfvcpnb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gxvhjymfm.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ghiukbevr.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gdapegvgm.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gmhafgprl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gmmtaxqsn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gclvmrhds.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gfmyusmkj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gkzzwqpdq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/giltjrjrw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gsfewapeh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gweqcsedn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/ggjtvvliu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gzsuftldo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gormymbuq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gcdnnyvww.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gsnbxqtbf.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gzmwfnqsu.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gnfdszulz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/giviijadc.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gxnnvmwrs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/ghoouzlsh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gkkatjoex.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gcpwtdthb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/glgvzfgmu.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gwwpsczbu.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gcrrgpetl.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gbtojhmqz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gguazastj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gvaoekdpa.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gxgsyxrps.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gcqbtahrr.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gwptguyrl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glyxdcvrd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gyanccvvi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gizduaurx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gebrvznio.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gllefcvgn.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gufnznvek.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gjgcqqiwi.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gdmitpeiu.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/goitnogdx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtutpulms.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqpcqncew.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/ggevaencn.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gbybyfdfe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/ggpnzljge.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/grlltzigo.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gbwebnbji.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gypzordat.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gmamxtoai.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gfjvhjtfx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/galcnyijb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gqbkstlkz.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/ggmdtanmo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/ghffskoxf.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gdmprkuzm.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/guohhjmay.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gqjeczlyd.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gmzlhsdik.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gqtqrynuv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gkwfzcenr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/glvdffshn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gohcgxdbi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/ggszfyadl.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/grcrsvcer.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gbzpolgai.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/ghldeenpw.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/ggzhvjjew.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gntxwnjjb.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gdglpygqq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gbpoiklvc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gjlxdmvij.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gienpuwth.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gonfgffit.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gzjaqksxh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gjokaaocy.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gmtbolwut.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/geendwvyd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/guhaklhvr.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gilepuief.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gxwmacnjj.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gyicobhax.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gwuxucieq.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/ghfdratxz.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmkiccrrz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gwtynpkqs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gungwtogm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gghcggjhw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gdfxnykqn.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gajrwkhmu.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gxcoeaftc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gdvqpoynl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gcrvbywtf.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/ghaqzydpr.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gzkbsccpa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gznbbbmod.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gsxzkiqzl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gurzykfwc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gxeqcpkdg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gfzgrmnlk.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gxtcmmpag.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/grtsvoqyg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/glyfygvnw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gxkkcanop.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/getphxdpz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/giewuunhs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/ggqizbkcf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gutitptte.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gmnbzljjm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gkqtdnasc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gvoxahyts.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gdgdiqflf.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gegkqfxnx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gvaoveafo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gjzhlrqdq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gmwuesdty.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gwfzhmopi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gifjmmrvx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/galxsestr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjgwvslvm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnpzkwkft.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gcdkahlly.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gomfgbzpl.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gwotyvuwm.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gxnfcqfbl.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gsqzuzgfc.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gzboyiczo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gwzvvfxxv.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/garkcmhzs.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gfwvqtpyl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gortwtkhz.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gluvghrmg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjvfsothp.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/guoammwbe.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gheqourgp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/grwmftatq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gladdvjof.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gsbgnoyir.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gdhaonwha.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/grebrexmp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gvamsxbja.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/ghwteaotn.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/glpzijlqx.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gokxnrlaj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/ggqkdomqn.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gokmthojh.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gwifmriew.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gxlgnmxfr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gmwjrbcak.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/grlbrhjnq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gywkgdarh.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gmwiixubb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gvpapscpk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gzlprywnn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gkkzzqmnm.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gpndtqgby.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/guxsetjsc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gffrbhxpq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gatwqfzum.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gquzlgmkj.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gpbnpuzpg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/grorpuqfg.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gkfwbmrvl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gfbuasksj.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gvqcqynqv.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gpfqejyck.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gvcelwpui.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/ggfmukurk.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/glsvkurjr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gybusqgxb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gbbrjwenl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gvovznhrn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gegkyhbmu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gdeqlpcmk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gmztwlfnl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gsrdnlvku.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/grekyexlt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gxnmxxsad.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gwekscyiv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gxedcyoyu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/grmiikyvh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/genxeqcwn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gkflgztso.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gnrzaeanu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gikkwjcav.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gjujocyvw.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gbfgbzswr.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gueeuqajs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/goyzwxzfm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gnrlrstca.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gyrrwgvhy.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gqwltvsin.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gohkvkxsx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/ghgolxswc.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/ggljybplg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gupstvsur.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gtasbukfz.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gebjclbve.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/glemozrsd.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gzepmywvc.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/goafsdbzd.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gyhtupsne.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/giajntuho.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gcnlfvhuf.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gvoaqqcag.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/geunzuyut.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/glfqoiiuc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gwzjvhwqc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gryzqslwu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gdjujcipe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gdwqpouuh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/giygiiyfy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gwnmwoeqa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gdwdjrlbf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gnvdzlyee.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gmdjpblpr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gcgjujrhk.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gvbuwehqd.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gghyosrlm.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gtesgjyrh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gctpkudvy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gkksjqpjc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gwiotzlpa.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/glkvrjexz.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gphhnbeim.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gyrrbeowu.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gkjwnopxn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gcctmmref.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gvbrsamnw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gblxjbljs.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gonoxntgf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gnzvfbehv.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gzqmgnzdg.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gvxcmlxym.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/glszlbhuz.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gbafgloxg.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gptzqhrfy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gvijhkznx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/grecqwnet.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gnhfiowea.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gdqtcuryu.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gbxuugtup.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gjwmrzfwo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gokdztimz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gtxpovhif.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gbuvxkygf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gymucqhte.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gvysrpzak.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gilvmjlcm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gnrmcnden.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gtpvbayte.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/guimqgqgo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gzgthusnr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gbgqvhatc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gpmhdwrgx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gtzltrbtb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gvaiptbnd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gekdaipvi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gfexndqbz.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gsmoqocon.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/ggrqotbea.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gwzmrojnu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gsyervllg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gsdhnddnw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gbzjschqu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/guxrnyago.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gdcskbmwh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gojggyelf.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gseplzfua.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gcbekwzkz.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gvjbmvoav.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/glslbaoim.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gvrxmvdcy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gaofachpn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gnpobevsj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/ghnvdklst.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gifjkjrww.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/glrdhamfe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gawtwtmfx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gbkcvednm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gwztcfxfa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gbdasmlqs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gzdglzgxb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gnicullrq.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gglvqntxh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/grdriwgfq.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gjixdxlys.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/ghebphdrv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gxjswyuce.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/goldarjuw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gpbyawmvu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/grffzgnyf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/galjshhyx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gwyxcmdli.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gpvbqxmsa.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gqwcuiiiw.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gktfwynkz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gzvwtnqgb.sHtML


<!-- 参考信息 -->