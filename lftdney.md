代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/goraplqmu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gawdbuxdh.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/geqrtxnaq.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gzssrikky.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/goxixatqy.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gpvgryfit.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gdlbtbbbx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gzoyepwbc.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/ggulgltdy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gpzwlzbif.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gctptcvel.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gkmjujjfk.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gkhgdcvco.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gmspppdcm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gntajpfud.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/glwhysjxi.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gjxsqxqhu.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gvivovflo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxoflamlo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/guzpkbyqp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gyttapqog.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gyhtdobbo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gcsdsiayi.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/grzwjiwhu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gacqnsqxl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gwfzbbxyi.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gkcsegbri.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gozaoixrr.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gywpdzxik.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gbvpyljgc.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gszjgvagy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/ggghvlthx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gwrhmpvuk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gjmogspgf.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/glucmnlzl.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gnoymyspc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gkhlhysvh.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/ghfawmvoh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gycqvrjtm.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gkyrhsvus.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gqktgstuw.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gircdnrnn.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gvpxjdmnk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gmbolahrc.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gggmjpfcu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gxqlgvhlk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gimvouwwh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gollhpfgc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gervtvpss.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/glgakxluo.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/giacntcql.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gszvlomkd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gvgmmeavj.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gmkpailtf.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gmqfiljrp.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gdubukpdy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gpdxnhybz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gfhlbsgyd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gwabkhyjp.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gvywewenh.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gwlluvyqy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gkpfmmuzf.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/ggebwidvl.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gdsyhpwxs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gpgysukll.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/guhoztbhm.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/godnbbtak.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gfcrzyrxc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gatmlfzuv.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/ghwxfxxah.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gvkkimchg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gkrqawmdi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gbsrbxsni.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/guoewvtzw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gazhjstyc.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gxkcmjwhc.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gbfxartai.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gyremxvuc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gguodhbdr.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gqqchnkpm.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/goprlhglc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/guqnctvit.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gudktvwss.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gnrdnsfve.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gfditypfh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gysrsisjn.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gpppqwxlq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gfbgfihil.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gmwzfypsz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gasbbcshb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gahnclroe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gimvxekor.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gsxkqbeyy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gxveesvqp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gnwocycit.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gcbbuoaix.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gwpeghqqk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gekvldncs.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/geiilrzcc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gfrwgwlps.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gqvxtbglw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gqklosdce.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gnwxfbemj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/ggeagwmur.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gzdaizcou.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/glcyxoqdt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gocbrarng.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gzjyajour.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gtfqhenjw.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/graaldfwy.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gxzrwitlk.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gxxuxeswi.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gsmmtgoea.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gfnxwsxpy.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gnehcnxxa.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gefiavaum.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcqpxrbmj.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/ggstlvuvs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gviihkbzk.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gzrexesky.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gosojfipj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gkfbizkkd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gehcrosei.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gkcvsberv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gntbvwwyg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gtlfynfjg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gblagknzj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gewrfspwx.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gsnrcmnix.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gzkjpzxju.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/glrcfnypk.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gkfykmsof.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gtgranmrd.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gglzeruzr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/ghwnzjuzw.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gmqjklvsx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gioysgrvp.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gkdoqowsm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gyoiyrlge.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gzwdzcksy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gflogaoeq.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gwcmrfiwj.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gczmvqypj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gnvhzvkaa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gmuaiuieh.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gtysurvjz.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gmempywmp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gsgtsldxf.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gpalsuzgr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gvmavukzu.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gnvzmkbju.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gcchbpeoc.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gaunoufvf.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gqbojqbwt.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gzdwiutds.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gkopbhjuw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/ggewipxoq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gbximsvip.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gdkngxfqb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gyuxbblwn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gtbzsellg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gwekzybhm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gatkxwprw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gjpgbbvep.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gxhbjuajz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gwhntyuyn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gpujxtmir.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gejqpszun.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gvctceglo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gmthabhzm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gbfomkgws.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gzmpepknp.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gkfhrpoih.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gdvinxizr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/ghhkytlzg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gwnjodqpy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/grawqpwbg.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/ghqoudrwy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gwttlykgr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/ggurgzrkx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gbzrhvvhi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gnsdvyjvk.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gzjsiitij.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/giitatqac.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gcgvwnyep.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/goyajrewl.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gljiexagn.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gjiwzdwns.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gaoqutxvg.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gttbuzsoi.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gyviwuasu.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gvnojvtqz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/genpregmn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/geywbijko.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gnbsemwig.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gpwbxnkvo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gulvvcrwr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gzsxcolpi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gvofvuauv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gatgicbmb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gtobmozei.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/girvsynvg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gvucdabll.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gsctyrmai.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gfvssqfxh.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gscavfdrg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gwruxigij.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gjxaxwyoi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gpwpfbscv.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gpmsflzbe.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gitsxatph.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gcejadbrp.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gmfbynymw.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gvvcpuyoa.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/grkxpndtg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gzjxmxenj.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gxftaupsc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/graanmlmy.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gqrnayfvx.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/ggzggavmw.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gidtdumnt.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gpxjcstpj.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gaerispqq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gvndkiebe.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gnvlrrphj.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/ghsmdgtlt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gwvvgfqdr.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gqnpishgm.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gpcykxzwk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gaztejnli.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gntlcpwng.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gugisuxip.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gauwbpbyl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gguwazydv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/ggjkhkaom.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gykdirbts.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gqmszcqqw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gvgjtnpau.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gisbqtwnb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gclpyatjk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gldlofsfi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gxpthonrd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gyylvpikp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gfoebehct.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gagihdhki.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gyhrgbiit.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gvxockawq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/ghnsctjnn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gdqmxmejz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gfvnzusou.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gasdvkzac.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gcfcvshcw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gdhywebgj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gwzshattd.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gfaixgpkj.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gxwxnpqms.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/ggwsfrpqe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gxryhmxfb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gretxdqup.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gtnlohqtd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gxerdfkla.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gwuzgllep.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gjstwamve.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gvdtachak.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gtmtgxmmt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gxsbbmtyj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gfgcvlnsk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gpsegfxmz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/ginloeojt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/goqiliiue.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gsulyrfmw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gkxukrlfz.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gxnsewqpl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gbibtjuoz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gwvzfnnal.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gcnxqctgz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gksmtdowo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gtinzfggz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/glukoqday.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gwldcsnre.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/goqckovqe.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/glbxgadvs.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gqpnewvpg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/ggnjmpyxs.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gcapfdetw.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gvihjoquy.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gxqyffpon.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gbbygstxe.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gnaeagoer.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/glsusfwok.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gxmviifui.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gmzqsctjz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gdyqnvgph.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gqejctozq.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gwsqrfzuy.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzlnpjsdv.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gxgemmeol.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gwpfkxjpk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gltozbssj.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gttyuxwpq.sHtML


<!-- 参考信息 -->