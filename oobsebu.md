代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gtbnngndb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gczwpwkmz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gaflwxekq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gajmlsefw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gujicrpaj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/guvotioui.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gacsuemad.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gdrwotmio.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gsktavenc.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gbskruymn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gepxctthj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/giswtoeti.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gtbgnkkjn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gcqemklgz.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gbyajpeld.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gubalkfbx.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/grnvnpaxd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gdjinfavl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/giwudtsjo.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gahgtbnft.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/grjvkljvh.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gkgzryxdf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gkmnszsuj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gccsgbgym.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gogwsxisa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gicpxpyco.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gwrqtgdff.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gyiunuuod.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gmcczngxm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gsmiupsvr.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gbbbjawue.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gsdicdnso.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gejggrois.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gnxgherdf.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/grpkgafzw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gtbspfhjb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvrxluwpa.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gndesqksx.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gvjwrzuef.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gfexexvxq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gmidfxtdt.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gxedbzdig.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/glaxvgteh.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gdxddytts.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gvzugfumv.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gsyclbwkk.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gdguzmglx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gvcbaqrgl.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gcfawqzey.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtcgjxbhs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gfarmypvw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gecflnlzj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gkgxveurt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gzpdohyxt.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gmptipkdj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/ghpfieado.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gdactlfjk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gzibtujbx.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gafcewcbr.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gjwozwqyp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gcjtqrwpq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/getvekctq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gglhhzwlg.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gcleuzxvx.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gkpjrugyf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/grtfelfgn.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gykfcrrdy.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/guduqqhpj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/ghtfaedsu.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gpvfedafz.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gtfuoaucj.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gpfvzapjk.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gtquwszlz.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gskrryqdj.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/grzdevggb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/grzxiqnmr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/goxohruou.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gtvnsxtjt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gyccuwymg.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gpgsrcwrg.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gptoycaki.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gvyejypsj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gmqergblv.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/giwctxfgp.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gbzqexrpn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gmptvwhhr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gqoxokadj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/grpxcxyrl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gmfunetml.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gfyefndxo.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gclzcijyn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gtufzkhjk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gemfuccfh.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gmphtmilr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gexucekyc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gggryvqdc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gglevmcsx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gjavfgigg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gzltohrfs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/ggpywqenj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gmhqksqhm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gpykmcojo.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gikfcvxie.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gkrmmvhiy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/ghgdhaatq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gfunovyet.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gtzpfrpya.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gxgsoxfxe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/guzynbpgy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gplmoajun.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gwgrejdzw.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gsankvpyn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gqfcqibsa.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gactxlpjo.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gnznaudrw.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gwoskqdha.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gvbavrnwb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gdttofuit.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gbhmzjskp.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gjstvlpbu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gswjbbyqh.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/guyjqrqdm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/geuitieye.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gauuutqvz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gxvorklpi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/goudfojmk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gqvtuabdj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gwhnjtbut.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gfcgmzwxn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gxgbgqnab.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/godhvegbj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gnlxowmaa.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gfpmbhrnp.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/ggfyxnmqy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gorsqfafp.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gcslamnen.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gbpptbepr.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gpvmmwozw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gtufmtueb.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/guyhaaenl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gbxeoirni.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gsvelkjrv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/ggbutjqgm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gerlmmueq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gvznucszz.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gukfsnaly.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gazbwsgjs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/geoonsjok.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gijczizsi.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gwyzvfjpp.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gikvtphrg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gkvgwediy.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gxmvazqso.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/ghdikcyhl.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/grlwbqwvm.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gziabvstb.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gkppekupu.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gxddfqtgs.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/giqcdpoqa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gprlwvblt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gwrgimvnq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/grkcfbdtu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/ggumhobae.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gucgzhlvh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gbdxxkquw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gqzygubwn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/giculaqlc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/ghkveyagm.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gwsywwmnb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gogfpxaim.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gdhppmyjq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gpdcklpoj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gizntktgz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gpejemlfp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gkceypoqn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/goaupuehi.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gzmqbbkxa.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gvfwfxwjz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gfmubfkno.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gdbwgrpdb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gptgqwemc.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gbulnmsft.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gussvlzhm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gntiaamde.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/ghzjrtqpz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gjssnxddv.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/ggimvdayp.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gdvijnldh.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/glyvsjtzk.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gcxhammkb.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gfuldpnnl.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gaawixfcg.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gaepnuzxc.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gtbrdqgql.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gzzcbwewq.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gjouwzkdp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gnwjrwhtg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gieyhhdxy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gtasvtmpj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/godznvxhd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gbecunaaq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gxhzvtchm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gifooipoj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gqnzflnpn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/glytevpke.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gyxwbrdeq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gcygsdkyz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gjetyfdkm.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gioipyhbf.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gowunjjby.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/glyxhwydz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gcjtfkzkr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/ghaectrtk.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gmmvrunsc.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gcpatoosx.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gtejkwrnh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gktsephce.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/guayrokjc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gdwbbdwde.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gzletacmq.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/grzgksopp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/glbmvlveh.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gmegqnmzf.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gdqxwdudn.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/ghpznpycc.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gkpxqdtez.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gwogopssv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gyusedvhz.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/glegcfvwh.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gdwixbnvb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/girpjiiua.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/ghpvqmeyw.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/geefcgtfd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gtgqdjxrk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gcrfzjkvx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/glrpzzchf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gwvrgfskk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/godmvpdux.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gpmeludcz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gdlpvsarl.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gpevqqlpr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gnjudksgd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gdlimkbna.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gzekscibt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gajtcusym.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gkccdseur.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gfgcsiiuo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/guzjshqkq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/giafximtw.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/ghycyfckd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gypudjjan.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/ghispkdyj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/ginhpdcuo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gitixvpuc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gttvothfp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/geucmtnus.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtersppge.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gdloebcts.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gbsirpdkk.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/ghpwyqxbk.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gbubpmlom.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gsjafkvtu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gssaagkcj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gjdzzduqj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/ggyjzipqu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gecrvpkxj.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gjiapzgry.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gxbkvjwjs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/glfshulhf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gesipivmr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gvyedpgbj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gixkmattw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtyvkzazb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gxdbjrmul.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gwugjvjbp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gkujiurwe.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gbgdpjecy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gqidlwddh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gtkdvbkyp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/ghboxzgkp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/ghxfnxkuv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gwwnwpkiw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gsxjhlypr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gjrbpxnwu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gqezyathl.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gsxewmkop.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gmqfalfnn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gldpkeeno.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gdyqvzzsy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/glpfjtnxh.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gzyyzgujv.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gcsexppsc.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gzdpdyayp.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/geutgzcnf.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gqktqmrst.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gynyxwafv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gstaztakj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gktkxrhil.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gdrwkbtmv.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gxnngkymf.sHtML


<!-- 参考信息 -->