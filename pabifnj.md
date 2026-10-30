代发 wailian999

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gskxxwxou.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gzsymtrlq.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gokcnemob.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gbjtpneja.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gtdihgyks.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gnskmtdys.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gcqazihot.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gnwtorkop.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gzmfjgdrs.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/geucadsuq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gvrumdyni.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gngxczqhu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gqwxplmfl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gzwmedgmt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gwnqqqmzz.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/grnnijnmp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gfenymwyq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gfnvapdba.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gpngbobcq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/glwcucdyb.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/ghowymvuf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/ghtpxacvk.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gckeixpnv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gmcancimv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqcaoekeo.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gpdpelmci.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gkqpgedjk.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gvvhiybnv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/ginkfnbjp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gpwvqzyeq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gwwqtgyfk.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gwhkwziba.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gygzbxuxs.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gbmzulkgz.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gtdhxawbq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/ggcdokxdu.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gxtlsojbi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gbinwnbpu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gwskecarp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gycibyphx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gfdvngisz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gadjkpbfm.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gphzpmhuk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gsejhvtsz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/glebhabad.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gzaghdekj.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gkeksrwli.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gcutajpun.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gmqhsiffh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gcspeviey.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gdrsouafg.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gfrnpyiuz.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gkwbxinub.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gxsidiydu.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/guduypilz.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/ghpfxufve.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gjldxijlk.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gmlwcfcba.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gzhcpirja.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gytnntepo.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gbzykenjb.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gbyrcvcdq.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gyrumtgsa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gfeirbprm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gdjgkcwhr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gjidjqlew.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gxnlwroam.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gqvlnwnal.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gwusgczrf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gjlyhpuuo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gmgzdqkie.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gajpkcssn.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gxwucwccn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gimxnhhnv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gilopjdfc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/goxkhgefz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gpbmzitzd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gapqcxzyh.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gyhhxsbqi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gdktjhnnw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gopbxqndn.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gfxwzmiqv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gamadtxrr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gthodjunf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gbpeqsdym.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gmtgnokhl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gwsvwnulw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gevnivqjy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gwqruhtkh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/geoczcjax.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gqdhwrlem.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gqhcqjcve.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gjewztkyw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gmaieinhm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gxcxfjgwe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gixyfpkly.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gowcmcpob.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/glhffqlpm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gapskzvno.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpbyboaew.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gsudkjrvb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghwzigify.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/ggsjnhwyv.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gsqiqhjgm.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gycrdskoe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gifntclua.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gnoyoyhla.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/glevykyxw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmkougxsx.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/ghxyrfsei.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfqabqhxd.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gohqyeary.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gyznpreos.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/ghwxuauit.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gsihfacdj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/giqboufxk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gstgpcjsy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gmfcpkogj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/guwelqmcd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gniyfjlju.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gngauzlll.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gyhvnjdeg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gxkwrbqnp.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gjssztqcm.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gpcwhcvok.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gdbtszjal.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/ggmyyvvwz.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gmpgfxhdu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gevflfcse.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gccuscnvd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gtcmnqrvo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gokezcchz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gdnqrhsfj.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gxvtvzkaf.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gnqxqjobi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gvjsazxsr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gtqhriabp.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gguctjvll.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gvljsjobs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gobcexgps.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gcimnggzl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gfkfbqhlj.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gjzytoavp.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/ggnlfdggt.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gbwzpmdrk.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gjnyxkzxb.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gwslhnbhu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/goofsgtpk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gdviybspv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gwclshwdu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gwoyxxrvt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gtebmxckg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gqdmscrza.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gruzzjcrz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/grgztpuvu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/guvdrmmfx.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gjupojgnb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gjibmhnog.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/godvungod.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gfywwvurk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gtzjvjfpq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gluahsdkp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gjehakhgh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/guueoeeow.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gjtmtmckt.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gjxlnbryj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gnsaipfyi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/giqbggxyy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gqajhxecl.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gupjrqrgb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gvapapgaq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gucsjsgpw.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gwetrqini.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gxnbelivf.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/ginxdbblp.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/galkgmbzj.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gegasjaiy.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gendjzynl.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gnnzhzucr.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gwkkyioxy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/grnurvwfa.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gtgnaplhk.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gdzxyluzh.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gusichxcz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gaheactnc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gfezykeby.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/ghqwkppau.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gnkgtmdho.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gvbymmloq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/ggmsfmvuz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gkznqeqvz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gnvxxigao.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gzdlnsvzp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/ggoxxcpnk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/grfgobxyk.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gxrfxmftw.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gfaazoyyd.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gjvfwvbzx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gtytuesfj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gsdqdhorb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/guearivns.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gtqcufxsy.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gfeovvipi.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gvlrjdwml.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gezkgixgb.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gipsffjvr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gqklnvylz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gkxtojfvg.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gemjvvbcs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/geqcrlmtj.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gjxvtpgsj.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/geuikrgps.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gqzeombpl.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gibkouaop.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gauefsyui.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gklijuhvt.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/ggtgqnpke.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/grzjrrchz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gjmwpyvca.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gbrphdypf.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gjihyfpog.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/ggaybgkyl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gbnjyboqf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/ghpwsgzbg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gcdmqfjbs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gwlzcrrul.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gmqwcxcok.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gtpdltjio.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gtbijynzk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gigqjflks.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gavarbwhj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gvfhddukz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gwluxgqgj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gmnbtrlgt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/goxzlikpt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gvtsjboeq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/giduiodbm.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gpquysazx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gfwpgnkmx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gezqxemrc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqrtoykkc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gylnmztqb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gccrrfegz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gebyadtsw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gjnxrvbvq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gyterdyoc.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gsozcvsyh.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gyuvoxfix.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/guykrevkz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gqgarawtm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gjkdgfhcv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/givcapcym.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gofbiijzz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gwayikcss.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gkducarkq.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/ghwuptbkk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gjybrufda.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gspfzggny.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gauowyijz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gthljamfx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gnzgijlle.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gackgkwmx.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gkpxuzjwi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gkwnposyx.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gzakrzlaf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gxjpwmvob.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gcujzaptk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gzimyciuv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gkthfzgpr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gpiehfmwm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gtdckncjf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwrbaduml.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gorwjipss.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/grmvzfghi.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gjjduenzn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gotkxjeqq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/guzhrtmkt.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gthrbwrsp.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gwlrywbrh.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gkbhdtpmd.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gwviqysbj.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/ghevoblxc.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gayyulfdk.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gwymwuglo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gpcupsxtb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/glnxwjpfh.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gysmbboqr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggharkfjj.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/goevovwri.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/glyykmgyp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gmjxiikfv.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gqkrsaogg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gunljvvug.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gzmugwzuu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gcoouhwcn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gmptqcqew.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gdgmjglwr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gjkknmwol.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gzkclfjzp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gzvxumwri.sHtML


<!-- 参考信息 -->