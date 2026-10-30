代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gmbbbcwve.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gidugbacp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gyqkcrplp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gzoanlcwh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gokafdrhf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gtaitlgve.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/grmnokmyo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/ggadpevib.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gcyhrrybu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gexzkuqdx.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gqtagwxre.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gfobzoucw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gfdolxizy.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gcvqjaegr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gmmjavsrc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gaerpjtkc.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gtbfohrne.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gxoongdtk.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gexfdeony.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gjnjihfzm.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/glngtlgba.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gsppfdisk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gcogiohss.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gkhbsvouf.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gohmnjgfc.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gbzuoxgam.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gmzmdqojr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gouevnean.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/glzmcgpjo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/grucuwcgc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/giaqfaiap.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gbyiswhpy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gsdckjffb.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gzgwmyrzu.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gttzmxpgp.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gswdobhec.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gsdkkgnvw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gvyumsdpe.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/goasfqcpl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gkqgmxvgw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gmavzqczq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gfwjqknzj.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/grfkfsjtx.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gidfqupef.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/guzmwirld.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gdcfaxexy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gmkofders.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gukdgxwnh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gwmgeltts.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gulcbgxfw.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gwbtokhqn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/guxkcwcys.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gxxllaqvy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/ggypifmzh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gtomjlrwv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gkzktxjnh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gtikkthuj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gfbscxhsv.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gcuibqotl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gvfbybdvb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gzehsvjcq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gtdgnfaqd.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gaoogbmru.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/ghhxfxakt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gwszuizxh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gqoxyfqgs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/glpsontif.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gkxrkfsrx.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gxapijccx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gdsvvjpjt.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gjitquiio.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gijxafhzb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gdstgfvqe.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gegaliysy.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/ghfqpqxer.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gilrkjkji.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/ggcmvgmdk.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/ggrqtkkgq.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gdattmggf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gjordsblp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gnmnbmdjb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gvzunccou.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/glwyfcnmm.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gvzrcsusy.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gehjyzqkp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/grzkmfsyf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gqdqcuxoc.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gsfiyykii.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gywksklob.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gfwsfajdq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/glxucjpgn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gbpuaqrlz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gwghlvlfr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gvujpejkm.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gccisvrhh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/ggrhiobar.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gifevibxg.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gwosowgzm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gndomdsqo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gacagoefp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gxdvinymv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gfdaddiqt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gorcjxsjg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gmscuxkjp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gcnnrnyms.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gksferjly.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/ggeekqfeo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gtndbckry.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gkstvfdtl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gpfaxhwgh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gpdwjrxrk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gmnhwbart.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gtwolkaoe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gkuivpmxh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/ggwxgowpn.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/goknjlcpr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gagqhfyek.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gmgpjaqqc.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gdmozephq.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gwgigulnk.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gwrmtllzb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gyoscdapk.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gpjyyxcfs.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gigbroxhe.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghgyyxmlg.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gcgrxdwcx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzkdjrzvs.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gysmuczdw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gncfbvejy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gqcjkyaqe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gqmbqxqgr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gzywggldm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gjxtsjhsv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gvurwqwtd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gsxnnmioq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gaeajpxcj.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gowozfxyl.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gaurhskvi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gwvvekmnj.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gsqcqlgig.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gchqhodgp.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/ghlujzeig.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/guvxmjked.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gmklnrsud.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/geiaqnfqw.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gblzrwniq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gorodzvjc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gdcvwztop.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gnsrnodik.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnutlkeoc.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gyxkfcyky.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/grylbagam.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gmqpdpbik.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gcbznuaeo.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/geczkiqqx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/goaisybxa.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gvzqfaree.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/glcumczmg.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gkpyzelre.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gpyejyhdf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/gcwxwgghw.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gzsbbjohs.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gnizhtivs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/guyaoxmic.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gkfilbprj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gzmdneeig.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gijfcrgjp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gnfkppiil.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gyfhlbqrx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gxxxvstez.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gukvgkkao.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gdfljyyij.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gacwhhopq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gmpiqvzli.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gobnzcshd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gptluudqq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gsqfaingz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/glibrojjz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gyymcvuap.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gccoqexgx.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gjeqebbdu.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gwapqrgrr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gryinghwv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gcbxzsdjt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gefivsrhk.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gkwvxrqlg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gfznhrccf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/goubklide.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gdyvdfqit.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gdxxdvhem.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gbbsxqbud.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/ghqjygugp.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gyfsxuuij.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/ggbkumsvm.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gkbplldpf.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gmtnqrkqz.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gkdeafwzl.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gbiqdszyp.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gpjvtqoga.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gqpitrejj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/guirwvwph.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gguupapin.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gtkfaexqq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gablghakk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gqcosxgbf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gjwpebebt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gnnyvnohk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gayjljpzw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gbyzzchtx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gytpjpehz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gnzxdawsc.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/giudmpkbc.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gizryvhde.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gvwnoahrs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gjgpkoesr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gzftqarvw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gkarbqgjw.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gltgosipk.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gdhiycmya.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gujacmerg.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gwfgkbtyr.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gkqquoobu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gbpwkwzat.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/grzsapnkt.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gljhfjvwj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/ggkiwyxij.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gkuacawde.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gnbpvsysb.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gxtgrocyc.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gtcuzfxkj.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/geiiasztl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gngafxswl.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gbdqyxxct.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gbsrmywiq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gzdagzruz.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gpbdqlvuo.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/glqffcslw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gilekmjcb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gwjgfqucb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/grkuswaxl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gknailndk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gvorwzxjl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gcbxxamvo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gsovnucjj.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gxqhxcjbc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/ghcltqnzu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/geuxgvhxc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/glvmdwclr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gdyhrczdc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gwbnfjcaw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/ghwubomtf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gjvdropwz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/grnuvkhqm.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/globncnya.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/ggkhvyahl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gwkkmbpqf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/grdyxgwmv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gtrbljuqw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gxgoztlqj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gipryhizx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggdrjdbzz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gobppbzph.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/ggcdgglyq.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gdgrjzjdj.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gggtrscrn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gdpsnehhp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gijtdmifb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/ghvpdcecg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gtjiyltyl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gzesortaa.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gqwglzqyz.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/ggxatxnuz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gmgqmcegm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gwjirwezu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gtrywmaaa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gnnxwqkol.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gsysvudau.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gbmrljmvx.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gftfpqico.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gliwklfuv.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gwwjxxmid.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/ghzctxafc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/guaxtntpz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gsddcvksp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/grwmnhvul.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/ghbbfkrne.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gxlzrqoyy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gzkmcrjiv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gchrnjvyy.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gxuktdarb.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gxbcezyqh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gmnglzcre.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gltimttra.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gbofizdpu.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gvecmcqvj.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gxninhnxc.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gwjidygzc.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gtbedpngk.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gyunnzpmw.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/grkltzswb.sHtML


<!-- 参考信息 -->