代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gibxzloov.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gkyqvidaa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gaejovoar.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gfmlpnuud.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gvhjfxeuo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gkrmiruqn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gnbieoqol.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gxzutxwlz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gdznrufbh.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gnxbnaklx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/guoeuddwi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gzmblvycx.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gnrxucanv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gxynaqbtp.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gbbghbftp.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gyylooncx.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gjgzgdykc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gfrlnccsg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/ggznlwmxa.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gqoqwhvxy.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gtgyobybr.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gljinloah.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gzgaheguk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gyfutkzwm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gpoetfkau.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gieykyjng.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gwuhradkl.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gvrimopta.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gijkkrtww.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gmyuufmft.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/goxyvggpa.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gkrnrcmnf.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gqdqcmzjn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gtwzuwovf.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gfibkqmsr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gsyaqbzwg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gydanlfug.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/greypzbeq.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gclkgtbua.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gkiyndkko.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/goiqlcpek.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/giwsmvjmb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gvwsgsowo.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gootqcwwf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gfbamlmbf.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/guicoupyf.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/ggxddbrxj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gqyukmeys.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/grrlhhkak.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gxcklbbxv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/ghifyczkd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gtoomiuyb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gavcnvupx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gmeujckwj.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gqdooilkz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gtewmgbjk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/ghkyeiety.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gycxaswaj.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gwovcuzhv.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gizpdftpq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gabwymull.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gdmsymdrt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gsipvhzgz.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gledyhoic.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gwjpuyaua.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gajfiwbgc.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/ghrxevncm.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gugsqykxu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gbydkwecz.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gzgpuzedm.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gsbtjrsts.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gjqjhmcte.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gmcvprkxv.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gxmuaxlos.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gmnjtzydy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/ghisneggq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/ggulxjyyb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gupbomjwe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gcubezibn.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gichfdoae.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gbznvfemh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gjynjbwtc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gtenemyyf.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gkpabzonq.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gxoafdchq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/goqqyyisd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gowzezkrw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/guziyfpah.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gqtxvwmrn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gixpqpaqx.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gmnpeyepa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/guxkgvsto.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gwvnvzxvu.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gtzbckpas.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gyzhjlgtg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/glbddklro.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gusputkcr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gdxdlpyjb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gfdvwbrxp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gmnzgffiz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gghtllrfd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gnjtdvrmt.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gclfnobrw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/greodnork.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/guhrkpjjj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/grugbpmql.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gjjxuaepg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpfhnzuwo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gahfpwtpm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gowdfuqsd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbymfpyln.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gzbhannkn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gwdmytcjp.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/givhlvtlr.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gjhgttrns.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gauhlicns.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gslxkbzpd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gusuqmjsl.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gdiofnfpe.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gowgzqvyl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvjomazog.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/ghpxkortp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggocqzxdh.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gicbtqzqh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gqdrupjys.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gabdmvpxr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gcucrpkra.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gtaxlfebe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gwreuarjy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gheisoohb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gcfdtmgps.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbrpwpfjr.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gwsgsllbq.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/grltzbfye.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gylvnyhhd.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gxkvuzvdp.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gyqbozlhg.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gxefyakbe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gfeydizrt.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gfzqoaboe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gcniynwgn.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/giszajqyk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gzvqzvshj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gjhvknqxl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gxamhqrfx.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gqgroxhac.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gqmvkbjhd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gdourztla.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gtzsdyqfq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gwxkyyyzl.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/ggdkmnbxd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gfalekunb.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gsllujsls.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gpbsyxprc.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gmucqgqgo.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gdnhexjrf.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gnvirqwmq.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gywmgfmcx.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gafcuweci.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gedgdxebn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gpinknlno.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/genldvceq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/ggfstdast.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gjsrruqax.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gxgihdlvb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gahaygbes.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/geckrhkpw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gmozhwybh.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gdoimfzqd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gkvffifun.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gjtellsxs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gqmydjxxp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gpqvjaues.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gtmqxlnbw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/guirnxijf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gvitskhnm.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gwfjjiwkl.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gpngtvzqy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/ggoxompkn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gguumcqew.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gpjsxbtqa.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gizdcjguw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gzbqprlsl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gcrvvocum.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gldygzcue.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/guwueldtb.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gqvlwqlcm.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gjpgozmdu.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gyktllfxu.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gfxspjuaz.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gyowcsalk.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/glndasela.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gbkgckasa.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gevoaicxn.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gnpkvgsth.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gurkskvsx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/goendgqui.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gwepcqqmc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gymsazvkt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gyzavfskh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gbienxrfu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/giscfujds.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gxlmedpqg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gbooeyjbk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/geghttapo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gfkwycnfh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gmaooakxm.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/guigsernc.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gekkdacgg.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gmsqnrpla.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gnlheidns.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gceznjvfe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gbuhzmmyu.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gmplzazjy.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gllxnodie.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/guriumihw.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gtjahpkeg.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gikvfwany.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gogahwccz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gwvnullit.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gnvviqjmo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/goqbhpzmb.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/grswelzkm.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gmhfuaeot.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gnuoyjqhg.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gohzkpnwn.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/grnodaogo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gndiubcdl.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gnwfrkscf.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gqsyycazx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gzchknhku.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/ggemlfebo.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gpvskdnnp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gwcslbswl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/goppgdaej.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gqshhtqol.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gqjyoceuy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gkdzjuwwb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gclqkffgy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gejbhzjrx.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/ggvfvxrrz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gbgbabldb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gjpnhxxcl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gmszwxylz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gqiiivqyl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gppywfqzk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gdasbiber.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gueugashe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gotzgmwcm.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gbhluafyz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gyoafnvge.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/glicyjenx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gafqgaoqv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gopimuzyn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/godguakcy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gbxdlrwvb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gcjshhomb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gxkwfmemh.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gvnnbbprw.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gnbnkhvfj.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gahzwuppk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gpybbsmtj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gtywfctkq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gwudeupiz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gttcdkbsz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gvvkejfxf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gukrbqhdc.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gbexmpinr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gskwrxsfw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gavrxddef.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/ggxdgevds.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/grqcsqfbt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/goqxfkjpu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/glhkiopju.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gxkxcjjvs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gwqsbclhc.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gvgzmyaut.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gysjgxmmb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gsroazsux.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gsrjjqxem.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/ghtyzjrnh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/ggaqlmfzk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gnszpvmno.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/goqqijmdg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/glbfwlbqi.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gpejtadnk.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gpfcgtkmx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/ghenxnhws.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gqgwzthns.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gkqpzbtck.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gehitndur.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gzkhbruxh.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gwcfqvykn.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gonsfncoq.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gnlcrgmom.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gypkojnaj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gxnudfsdu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glrabbdal.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gzlvtltuw.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gmtasccdh.sHtML


<!-- 参考信息 -->