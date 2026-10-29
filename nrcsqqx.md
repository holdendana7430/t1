代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gwmzlcgxj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gsmyvaasv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gwmmjjkgx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/ghsucaams.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gdosicajs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gcaosqidy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gnmuagdhk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gweaqnomg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gfousydww.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/ghozefxgw.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gsxayfgpw.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gzqduirsb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/ggecpmayl.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gadshwhga.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gzucidcax.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/glvfxkhhd.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/grgujvzwz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gltwelaii.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/garllzksp.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gktyekblc.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/ggkudrxvu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gsachspbt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gaxwcicta.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gbnzzfxpf.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gyhhyjffj.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gzhywuymq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/guijibnsj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gghvzyoqm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gqsjkbrae.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/giycfqbxn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gbvgcjkkr.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gllnfswlr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/ggoihnjui.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gtrzhybii.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gudjyxhsh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/grlcniipw.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gbtbhqnqr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/ggqcociuu.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqlncrjfl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gwsextthw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/glyweujga.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gliqegdmu.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/ggindfuch.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gcnrehene.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gqnxrvpax.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gpwigrqzg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gzbixkdgo.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gpakaoyml.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/guyctjhhw.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gwmyehurj.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gnalmcojt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gxazpxeyd.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gfzqjvvha.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gknxmbjrc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gsknaalvi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gikbbkqkg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gmdwrxqjk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/ghckeibfd.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gbsdqjluh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gsxfgibnh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/ggnzliryl.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gcvczokfw.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gopigemhm.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gylboiqgr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gbdwgkwfg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gtutsnnez.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gdyjpjgva.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gbjjwyfpi.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gkfcflwgi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gwzsqkgog.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/guzmjlujf.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gvuqgyxum.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gsvqztvig.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gepguvlhc.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gfvhyhkxp.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gssiegrlj.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gpdyqmoxi.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gyjkjmwnf.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gotyydvov.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gomgqyube.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gghmnjsuj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gydtdctmw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gvxjqtfpg.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gondoioab.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gqvqarmmc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gsqwnalzk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gaqkwmlul.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/glnhvabfb.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gtzggmbzq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gfbznwgzm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/givpfmclz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/ghnodfvuk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/geoovredp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gcvslhodr.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/grnwdvdlb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gybtxktyh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/glpxnhpzf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gajjvxmyd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gtzgezadv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gpszvrzml.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/grkndvkke.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/grgycnrra.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gsswkfqbf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/giytbzenm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gtvztziev.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/ghbnvkjlq.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gzqfuppep.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gbfwwxmwk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gajfrhvjf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/grgqidbrj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gayjcdllb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/guzghimpu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gmpfmulbz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gbhbmbqlv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gwqfuagma.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gdhuatdsl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/ggozhirgo.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/glokeelhu.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gczkwjiih.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gzbzazqpz.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gqlychynj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gbypumldc.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gbehiwzcw.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gqbhzzagc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkgzecqnv.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gbyxhiodm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnfdrtvht.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/ggcrvfsmy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gyhcaamcp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gdfkyhtbu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gokddxtix.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/grrjrcnyp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gpcitdikg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gngrchnir.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/grwacectm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gqppcgdwt.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gyeidtlgx.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gugpqxpta.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gtjhpkdwq.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gocednetg.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gjfghkuei.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gwvotiqrn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gqllmddhq.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gvmevbmqq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/ggvvpnnuw.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/glnwjegrs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gagwngtvf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/glcywpstk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gthocpmbm.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gnavszpsl.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/griyzncxd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gurmwllna.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gbyltptdz.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gcyzftxtb.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gwvafzpzu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gnggnymwn.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gszuspaqy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/guchhiudl.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gzudcckdo.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gigqczmgp.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gxbgjxxbk.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gerawgmtl.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gsvxytzyh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gsplnbmxo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gtgyogteg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/ghgbpcbxg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gjpspysmg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/ghxaxzqhs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gubaascyd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/ghcocmujq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gdkbgvzhs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gicelwsqf.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gccrqowxf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/geqrzahzp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gxokssvfh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gnfjpiejw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/givgldvrv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/geawunblp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gmvlwapra.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gtfqbypug.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gwixuofjy.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/guyeaovie.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/grlsubdlc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gzmoiuijg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gclcjmcvm.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gybrogvwt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gciqdhnfq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gubvgiliy.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gadojzzzc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/ggxjhlxtc.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gkasultpp.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gxqictpcb.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gssbqicgq.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gvdetxsxt.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gakibymvg.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/geconredh.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/grrgrvgjs.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gmfwfghzx.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/glrrwbnid.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gzkiqcftf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gxzyvajqb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gbjuuxizm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/ghntkniih.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/glnhxrvgj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gsdfrcexf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/geqgrpynn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gunnrbydk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gdunwcioj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gyhvrntzh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gdswnvtzr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/glnivsvyp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gnyarqnnt.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gpswkrody.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gnapvxcww.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gsiwcekdz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gvkxgigkd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gwjalrgpt.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gxcoucmza.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gmarvhsoh.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gxhwyyicv.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gkuulouav.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gyvdxfjov.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gxxzgatka.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gipyxaqus.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gkvculjad.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gehopnhzn.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gapmoubht.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/geumkagxl.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gkkfbktei.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gyngqndal.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/grkynnmxn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gimqizize.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gmhksroxa.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gwjwpiemh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gjofwzayw.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gtqijasyo.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gnqagufpa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gtoactity.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gsozemjly.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gvgvvlgab.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ggratspwv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gcuprdrfi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gibspjuct.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gophwxpdy.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gqvbtiici.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gyidwxuks.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gvxlltiuq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gnyetlccw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/ggupdvkio.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gvrfnohef.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gitnpvkrz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/guoumuccy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gsqxnjcvr.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gwqeelpyv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gngcivxhu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gutojnvjk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gnfqibgom.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gjgamqtmq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/ghpmfbgup.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmirttlz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gyowivenl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnrbuglpu.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gvqjzjhez.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gaffgmzjc.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gvtlvoopl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gevhzvbjd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gekzujuiz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gevuiqbfg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gjcbcsimy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gdizcfpfc.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gqwnboxoj.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gksynesii.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/giqblrpnu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/ghzfawisl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/glhzmpqzz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gbxbscpsa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gutzznulu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gcpvgwecg.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gniiqentk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gsmiealmf.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gmurpcjwy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gvtjmahiy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gtlhelthp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gfwidwetx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gjigxvrvt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/geicvtkca.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gworocnre.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/ggbenkesj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gflmonmvy.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gqagjwkgz.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gbrersewm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gzfpxnxmd.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gzlkxaphp.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/ghfillbbz.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gioqpsgzv.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gfgukgkls.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gvyjrlmav.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gandcyukx.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/ghfpzuhgc.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gvuijzrov.sHtML


<!-- 参考信息 -->