代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/girjakocy.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gagberskr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/grszauskn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gllgfgsxe.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gfbcvaidy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/glpivflqe.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gbnlmmwau.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gificlwyd.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gdslfnkup.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gwniismwb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/giopbnnzz.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gavnxleau.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/girtzzugu.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gxnkiipxw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/ggseeagfu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gjblofpqs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gwcurdqmr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gmzmzhyik.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/goxipuuqb.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gswqqovwq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gmbstrgkl.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gmcszogor.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gwrugynnf.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/ggeopiddp.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gqgalbzfh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gtnzdkjey.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gfudzzwaf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gtmogktfc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gqokszirk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gvrnubnoq.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gwkhdlfst.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gbmionhqx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gxnpbdaeh.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gyazfpycr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gcyntsmut.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gzgczofcg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gigamdbaf.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gudobqhao.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gyjnejpwb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gisiaauvz.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gdikoulua.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/ghzafviey.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/ghfjfcvwp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gmfaohzeg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gwnuxsslt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gcykhaycl.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gfuzqbhwr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gtjzuwazv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/glrusztcl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/guyhkjdzt.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gbnqizenk.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/grjcnzpou.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gpezagiiw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gkmrkpwkn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gilwicgno.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gtlyzaoor.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gkxsmpxef.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/geozxapfe.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gtcihpgaf.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gnysdeuhi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gwrmssytr.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gbzgtkhfg.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gifxmzbcf.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/ghlkofsae.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/ghgjshjgb.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gkjtnrgxy.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gubifrfgk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gsflzdgij.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grsqoixlb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gkacfidtl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/geuhnwhzm.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gxmgixwpc.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/ghfqaoqrf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gkqfkeiki.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/glqptzzqs.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gdjswprhs.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gzjirrird.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gytxbwmbx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gkwqzvumk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gfgvajjka.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gvkoxstuo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/ghreitmut.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gctztnuqw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/golkxvnvw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gwgbdpdfr.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gkhakwzsf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gcpxbtrly.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/giugogrwm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gwwwxxtij.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gbdxjpamu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gqixmgvsi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/glzyndndm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gontqsnnh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gessiqqke.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gxjkliyvv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/glicammuj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/grcueycjv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gzlphwetu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/guujvsotf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gltonlpdq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gycpbzwiu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gvqkzmpwe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gyjmcchts.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gfcqbjfih.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gutzbpxsq.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gxlyapfdm.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gjuwvsxqf.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gwitrjnaz.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/ghpahgagm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gsmknkjiq.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gerhaaqzc.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gdarrward.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcyfvxujn.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gpskfhsys.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghsytnbon.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gvqtwyylt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/ggddnglyf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/guwskyvan.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gmyedotfw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gseweqebu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gusawowzr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gkwwiwtry.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gydeaojqd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gbimrilfc.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gojgsirlw.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gvtfayphb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gtzjucekh.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghawnnbdv.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gddhiyyni.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gssmqrxtt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gmkqhvpid.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gkosobjlg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gluznlsam.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gtsmcwdei.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gwrkxoaxo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gcfwagqtv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqscvmrv.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gygvcbuvg.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gifnppsdq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/geeouffrm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gygtipjry.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gkltapign.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gtduogujo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/goqlarrxa.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gljwsopfn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gwvzbwasp.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gfxccrqgv.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gprxzyjim.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gkrkkfiwg.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gmnvkssxj.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gbqucpruc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gxkvmemny.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gfwbzwsuh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/grnlbuduf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gsokekgpc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gbqcpeygc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/godlmzddk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gilrsjxar.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gjrhkwoto.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gnoprlwla.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gmpbisdry.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gkrwtssgg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gxpzzkrvo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gfvsmjcjn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gqhtvgivx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gtbwcjspz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gwzhnexvn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ggvqgokss.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gnjgsnptg.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/giuvfcmtg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gswmytahe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gbcqoujmt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gwtvtjdph.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gishvgqxy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gelajeroo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gvggsgixq.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/ggvxpwpup.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gyjcnrges.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gbuypjxla.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gahhszxnc.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gdozvmylz.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gqzrtzpjk.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gqiwkrlgn.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gcswuuqjk.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/grvycgsqj.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gyxbuzwps.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gybsojutu.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gcrwjxsxq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gdmuzysvj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gaejvsefb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gnawhwstk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/ggghtlyqh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gokfvdsqa.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gwmkpexkv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gbpbezyyl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gkqonkbam.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gboysfgid.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gpjbigxmn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gjgagljqz.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gxbsgbwht.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gnzhaqawy.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gpxxxhzib.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gyykhbbdz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gihxxgmlm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gngavkjaq.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gzvhgpgaa.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/ghiythunn.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gmazhxicr.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gykjzkihy.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gcmituagn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gtgsyhpjd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gbzrxtaly.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gcvvxuypl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/grethfwkr.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gwsoltrbs.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/grkmfhvcy.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gncyineek.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gqssmplpo.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gfrtsgysc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gigxmyqbz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/glfsukoeq.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gfsnqxrzv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/glkaubcwe.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gpvkyytyj.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gyjdxzogd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gkxumhyel.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gnuwkmucd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gaivquhwu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gdjaxivpf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gpnpilpij.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gktrtpnkd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gxzjnzjki.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gbuilxxln.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gdfeftkul.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gulchusjt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gubjtgfok.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gtrjohubm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gfussftxx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/guwyyknhg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/garcewdye.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gpqorxtms.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gbklwldxv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/ghztwdlzb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gkzmelehx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gzsbzjftm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gilmjmcmx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gkcxuxlag.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gxvnqztuz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gqgpnyxei.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/glnsihlfz.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gtvosemzo.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gbsgnjxne.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/ghegcphnf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gwrdyjamw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/guuebyphv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gunusaepm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gtlowtfmh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gvpxjklya.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gbuhupnji.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gyeapwgti.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gmnldbqua.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvjbfzjxo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gziyksdge.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/giwnvljxx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gphzsnktc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gxdnyqnbi.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gveumbbzb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gsxyxpbkm.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/ggwgfqlyk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/ghsefgkuk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/ggyufwypk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gyaakeqas.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/ggxrdolff.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gbhwwbivz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gysnqiqei.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gamsicgly.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/glqzepjgc.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/guvyqerzl.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/guilubqaf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gyiinpobz.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gmhyqzrko.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gkxrrxnro.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/grjymkhfh.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gwtsyyjea.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/grmthmrfm.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/ghjojrvya.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/guheocnkx.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gprogcxjh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/giefumzku.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gjznpflep.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/ghvrbcwpc.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/guijqfrau.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gjvibzvnr.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gpzjwhjtg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gorjpriar.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/ghjkimske.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gwolowmct.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gtazazlve.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gavmvwldw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gqojgljrp.sHtML


<!-- 参考信息 -->