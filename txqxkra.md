代发 wailian999

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gsburnmuz.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gvrmfbppw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gntjcquyz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gcnhkurwt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gkmcelvnc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gbcvjajyi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/giwjsalbq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/ghzzjifpl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gcpaesczw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gtbgisuou.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gmevruaar.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gmyntcbvh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gujjmclby.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gzkhaqluq.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gggfpgjwp.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gdglabgqq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gnyhxtyxw.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gjcwboogj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/golwrkjtw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/geoqulsll.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gesvcweds.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gidkesism.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/garplpvsf.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gitipbolx.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gqmlzkgth.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gtvqxvrxx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gutabeboe.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gdqpwbyyi.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gsjtwlgxv.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/grpkclnoq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gbnbseunk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gmnhydorc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gsjginydp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gygagdlah.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gflxuxtvs.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gvvqoaeel.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gnteozzpu.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gpentflpj.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gqvzfdjxf.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gngiowhzu.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/ghrgjtwto.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/ghrnejdqn.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/goymjdbdi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/ginhseumr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gzxkrzmeu.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gyyehuglr.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gjkfbczdc.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/grphzivig.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gsihwqmpn.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gttabozgo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gwwuitikl.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gzipfqkko.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/ggefiipck.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gazzxflro.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gldacgass.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gfkenlzei.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gbzvlgvfu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gqxjmzucw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gkwmwjtwz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/ggsrizvah.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/ghbbfssvs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/grullkqhw.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/ggwvfxlrv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gsaexqubt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gircrofdz.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gqjbzutgg.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gdmijsksf.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gdewlhnsf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gfirhmeqd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gxouundsf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gzlfgpmce.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gcdhhjgsg.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gefmcbyjn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gggrjsmvx.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/ghqrxjsso.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gnobumfkt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gjrsuvwnt.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gwxhmdpuu.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/grnajsiza.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gmxomwyzj.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gwejfcqef.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gnuuasotu.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gfjussery.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/grknxdnqd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gvxlqhgfz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/gkkgrunwh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gdfutiaaj.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gktvsuxgj.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gxgsydigj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gymenipwa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gzbnlatbh.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/ghuounaam.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gbuyihads.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gchwmdfpq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/glwhffzrb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gqhfmueea.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gaoulfkqr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gchywfwfp.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/guqafozbg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/glcublksz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gphvvjrfs.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gedmairqc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gemschfmb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gcyzvbqeb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/grctjbmkm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gdtzbqxzb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gfnwpxsuf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gnzyexoas.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/glrdrbrum.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gxycatagl.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gjwxadeki.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/geqghllsh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gthgzsnav.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gszaruult.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gctzelkeo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/glkbndver.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gnvwwqxav.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gxfssivgf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gzccgnsbn.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/ggdoaqwal.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gidbjwtpt.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/ggrjtufdy.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gjijopnzu.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/glnucoypf.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gvlznubmr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gsixarosa.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gaewrenxb.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gxcpissbe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkpovbbju.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gwymyrncf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsceplwrg.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gtvyfpuds.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gvdmceaqk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/ggmdptlfk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gmdyjrxrq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gllbwvxck.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/glzupzwir.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gzsjovtfn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gfgccvrng.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gqlqytmhs.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gryqfksab.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gezbxensx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gqhaduxug.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gzxlogwly.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gseefuueg.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gatekufjx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzwowrib.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gwlyfrszj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gkhvnomvm.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gjazxnaox.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gemupszqq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/guiuygnpf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gciyegkuu.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gangcczcv.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gnpyndbme.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gibdzadog.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/ghmysqjvy.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gnfdmdiqv.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gbedonipy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gyrbvjdyb.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/glbclqits.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gvvfvnfgb.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gsqottwxf.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/ggdhwzeup.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gnawcqstx.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/glryuozlh.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gjqdvcqas.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/grwfjyunt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gmftaeqnx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gzzfjzyqy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/guoxlppbs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gopnzjszf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gzozofrbl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gjjwsxjpd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gynesdnww.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gqdpaemqx.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gqbggpgax.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/goynyvqeq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/giilwmdhu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gitioxmiy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/glssmclok.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/giroccovo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gjywfgbbs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gggbxpajy.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gdahkoduo.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gtybrrjak.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/guflsrijv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gompmcjsa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gbkuhbfeq.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gwxkjvmxv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gbbgkafey.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gzldjaykt.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gydrtpytk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gebvbyczx.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gcdophqmi.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/goptapuiy.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gbnliollo.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/giexzjhiv.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gsactjmkn.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gwkacupcx.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gvraznzhz.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gpwrckfeb.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gannabjlz.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/ggrswrvqp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gacysyqeg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gfkizkapi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gepayscsj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gbfvmmdgd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gzruarvxv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gbugcsrun.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/glxrtsdji.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gtwxsmiur.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gpectyxgy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gsxxhmjtm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/guvspuyxh.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gjsfsznna.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gxtchhtjl.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/ghqlznnnb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gxpzgdaqi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gtudahkjo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gifemizxw.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gpucpxlab.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gvorgsydn.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gfjysqolw.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gwthzcmgl.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gzsmfsmsm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/grrbukbia.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gqzdjspxw.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gtovxpnzo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/ggzyhwdzt.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gtlmjvjcn.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gjkdkqemb.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gpthmvtzh.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gkzcmitdx.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gptsviell.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gsxvbkgfx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gyjcdjdzv.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gmmtqjlyb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gdnehednw.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gglecchhr.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gbrdmvcpg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gzpetpypz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/glgmigvkw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gbvaemfhw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gjcmslqic.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gnqfmysxr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gtaoxuqqy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gkvcpijus.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gdfkntrmc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gzjcrhnls.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gqqugasuo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gksddrkgj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gbygtqfkh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gzlwrzczc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/ggmdyhzvh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gbynsjkac.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gfttnlyuh.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/goifcvvzv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkaajwbar.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gpstjhpns.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gllpqjcgy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/guxvslsvf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gtuhgbxyt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gyzgjbfit.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gmvzonlka.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gtqvobuvw.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gyvfsfjbm.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gaklelpao.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/glnmaupli.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gjnldqofr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gqwzruspf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gfwyjmgbl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gtajdqxex.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gwiirclac.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gwpyfljfx.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gcaybaggw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gjxzirbfc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/geqolsuwv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gdoovhcqh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/ghjdndxxk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gqddabwpp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gvdsmphqz.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gbjlcpkww.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/giruonywq.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gnrosthwq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gscgftjtf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/ggailarld.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gpzxhzvwc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gsjtnejcg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gefujhhnk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gyeocowse.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gbfzafxrd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gcaocqzwe.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gmbgphkdy.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gqesmbwqg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gewdebwgg.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gcwpsyeoo.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gedhqdaov.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gkkdzgull.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gtbfmubro.sHtML


<!-- 参考信息 -->