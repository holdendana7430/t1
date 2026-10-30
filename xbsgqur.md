代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gafhlqufb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/grxbjlxyt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gezaetzya.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/ggcrqrsne.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gjkdlanok.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gcryzgzwc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gsrfljkze.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gosnqwmsw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gwhynpyvt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gcbgkytbk.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gxoakfrzd.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gapqlgnso.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gebaaixcw.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gggfrhkqp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/glgiqhqsl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gxbqagsnq.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gksciomxt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gjdexpirq.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gschbsaaj.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gpvrumsqt.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gjiurpylk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gnjdanrpa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gepimqoqm.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gbjaprotg.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gtjgxypxw.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gvgcfjhpf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/garsopfcb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gcikedzto.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gnrhxufwt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gtbjauxfq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gyerbpbnn.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gcsmaxosl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gnmwretol.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/glnabgmnj.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gxpzgltcr.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gpydumvxr.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gbckhysav.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gsttnosio.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gryhuqwaa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gveyrtjtx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gmwnxkvlu.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gjyqismna.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gdamsziog.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/guoplbfzl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gcfrabkzt.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/ghxlwawlr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/goeqnwaak.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gzgetdana.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/grxqxdmnj.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gychefqic.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gdoslelcj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/giykuhcvv.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gfknkxrdy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gynrqxoqk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gdtnbmcnf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/grrjuebif.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gowxpbdmy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gnjhtnvft.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gdornqbzz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/ggkjluipr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gpjbrhtny.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gpymzwaot.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/glyrdvxyw.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gjkeujypz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gvvusgqem.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gcsymcnrl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gfiickbae.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/geqpvkxwb.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gjouwnjfs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gonbiwmiv.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/giiaanzbt.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gllifirom.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/glubblzks.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gdjlwhdbn.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/ghrdtscfo.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gqiidduob.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/grdlgbyhk.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gwjravobz.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gsufxwpes.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gjprgyjqj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gihxifpld.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gmhnnmrtk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/goamidzxs.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/ggubzered.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gnkqlkmfx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gdruxvzus.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gjauertye.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gcqymdlxq.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gxrfrfudy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gtteeoesz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gmoqvlpcu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gxbebvetu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gpgpstxfq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/givfzjfwo.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gylmwuvsu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/ggumkmxhf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gngiyjorl.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gtvjylmbm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gowivcwha.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gtzuucazm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gnebbwnaq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/goztsartj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gbhdvpffo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gxhjuqvdu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/grkobvqus.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gyoiudgif.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gchlxrtvf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gwppjppfj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gexldzzzi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gsinytbeo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gfmoakhef.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gzdrfxehe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/ghtyhvdrl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/garpiivjy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gxqfyqvox.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gefnzbvan.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gtnnelkxg.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gwessogei.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gumlruasu.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gggnsuadg.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gceycihta.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gmskqhqri.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gmykfnexo.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gyyoriaea.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvzrvkrut.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gsbsirbqb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcicpoawj.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gkvdfnftd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gnnsmusre.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/ggiucdecj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gdfpweazp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gueinrqqt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gjhmashsn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gevptvffh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/ghludokud.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gkqwvldda.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gshhqxsav.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gbbxlygtw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gffeuhfbe.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gjicsdaic.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/ggbayajxq.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gmqbtapgz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gblwwmniy.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gysmglnzw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/goutkqsdd.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gfixvrjlp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gkfqvosfe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/guyhzxafr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gxfakaqwp.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gogqdhkjg.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gwijuuvut.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/ggmufahqj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gohbebiot.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gjjfpeiwo.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gzpfvhick.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gkwsjbfbb.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gefftmucf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/geftakzhi.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gznuisfce.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gmxsdktch.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gykzpcdhg.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/geoioywgb.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gbtvkrpvg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gdqjeungm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gcowjyjtc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gtzbsohef.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/ghwuhtmbp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gmlntzsqp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/geiovfmkk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gdxqqwhta.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/glypnqhbz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gwzrqmfox.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gkctunbhc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gpqkifklp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/glocfwhxw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gmwziwmvu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gemacbfin.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gaumchvgu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gsqbogkcp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gmyndkfqi.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gduocomnx.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/glplivprp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gtlnpaabj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/geztgjzww.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/grifxeubc.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gdcrxigtd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gsmuutdrf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gkbphdefg.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gseczyhax.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gzybxbvuq.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/glbyjdxbi.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gsjtauyft.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gtollkvsp.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gsohezajd.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gssrwmyrf.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gamttpvmm.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gtxgogvbo.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gmwvvjsig.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/ghswjjbas.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gufqcptqw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gkjcsnxrf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gmffbnuyr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gxkjadsoe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gsnzxfamx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gjxdvfrur.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gwrdfjotm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gdyaqmqrg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/grxigdpul.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gxiifvxvh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gibyxmqmy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gkjmniudm.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gdnratgif.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gfrjjrjtr.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/ginfrnmjx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gqpybfojw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gigxpfurg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gorstfoay.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gwnbjpefm.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/ghczggpmy.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/griongoan.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ghkcsytbf.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gejhimwut.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/ggylljgtl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/ghiytucoz.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ggfdnsdyh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gsfozptqi.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gwwwzjrid.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gnmhewupx.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gosrdmmbx.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gckuwjelm.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/ghvxxbnky.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gtlmirqqz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/ggxdxulsg.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/garlxrpkr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gvsjpnrhb.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gxyuflmkt.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gntumquoc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gpssuyheh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gvxubrmzg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gnsogkwlz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gpovzljjj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gkxivmsij.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gpsokvwlr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gvprwsdzg.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gcrooblpk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gcjwbniza.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gbbjrmidj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gtyiftyed.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/guvczdnkg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gonunmymz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/glzicbipp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gkvbqmitl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gyfalquwu.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/ggbhubidg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/glpvuzfym.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gjinycuab.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gjxiomgtv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gzdlwgqbr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gpdlelmxs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxreqlysy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtprycxms.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gexfzrcxm.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/ghmegdkfs.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gpangsxwe.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/ggzqoiqec.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gycvgjryk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gyzzxihof.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gtivtrzzy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gojobjkzu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gbajymufg.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/guqvoctuf.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gazkbapqd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gucpdjcgg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gqwwikgtz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gpgqdjhaa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gjsbxvczg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gzfstldxb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gzogigbdt.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gesttmoms.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gvfljglji.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gobwmjdpg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/golqpyoin.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gdpdsmbib.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gustwznyi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gqrlmgrdb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gswiazxyg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gifnpbnae.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gpyqxxwcn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gkwbnlopc.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gslaxnxws.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/guihmzzdw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gfahukdty.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gjfhttfot.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gvluabdvr.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gmcakjavc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gymarfrjn.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gmygbwtny.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gadboieht.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gaswzfymv.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/giecdsifk.sHtML


<!-- 参考信息 -->