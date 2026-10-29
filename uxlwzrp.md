代发 wailian999

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gewonwcrv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gzmlqqetv.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gvjqufzyn.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gftlntznn.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gmrlnrqyf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/giwqmfhwb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/godtenpdm.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gmnhlgghn.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gvmbeeqrl.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gnaukmdit.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gifbxdfkk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gqxnmrizk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gklqaaxtt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gpiibooln.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gqgxvsnbm.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/glsuwsrqn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/ghkdfzfns.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gnxucizcn.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gyugtmiks.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghjvimwmh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghdjzqrwv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gwtfluhif.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gjygtzdez.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gkgahztgf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gwgqglmlu.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gpkszurbn.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gquacfbjb.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gmybecgde.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gbciffzvs.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gaisfirtr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gfwrckjit.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gizbzamqm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gznhcwijy.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gjweewjpv.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gzjdlcmdz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/grxaqciba.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gtydjceor.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gvxsliroq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gtijhjpcc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gxkhykuwa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gednsrjdv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/ghgqjsprj.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gsdbecpza.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gmlsohzst.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gfpoenrbn.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gbgnujsia.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gmxrvqkxf.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvvoalclm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gkopfgdyg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gbkcejqtt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gtuarxfzz.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gngayjtcj.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/guzemlwko.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/ggfnjvpuw.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gatdzuuvi.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gvyalkyvc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gjwalyecq.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gxusunvcm.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gdbtllhtv.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gztbaiifk.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gsdmvpqvj.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gjwiggkgb.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gzhuscxhe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gbcsuxrzw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gksrptwsf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gvjxenqry.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gctjejnmu.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gtwwvjovk.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gfvnvirpe.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gvzgmvgyl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gjhyicawg.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gqsymbyyq.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gqsfbstqm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gbeshlrao.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gryczsona.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gvyenqpkm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gceudvfzq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gmydocfou.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gqajbtato.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/ggyqltpcl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/glesknnmu.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gizkoprlg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gtoyboekh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gilgojlic.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gihnuqheq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gkqikdgot.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gjghhlput.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gcylhvbwi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/glvaktdez.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gvlcelkyf.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gjueriaiw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gbdcehqbk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gkgbxqibw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gwcbbinwl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gfxhswucs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gvkryukub.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gcuzrzmim.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gyrucqomw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gdejadgfs.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gcysawopr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gibickbsw.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gjfreidwf.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gzqnpxeee.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gigezonuj.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gxzhrjzdj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/grcyrwwtw.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gcgrcoing.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gkrvexfsr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbwhufovz.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gjsfsukwu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwudcweby.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/geiawdfsc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/ggqgqztum.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gtsjdaiog.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/ggsywmrrq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gxlnpwzqr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gqycdnjsw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gjyngxvkp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gpaidmqyw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gykgxeval.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gdnnayipn.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gjadjvtfs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gevxoblmv.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gxyhxwvyp.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gbgykfmvw.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gyyhybrgr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gdhfsngyi.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gcsprjwbc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gpktkbzin.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gbmnvandm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gtxxfhxoa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/ghmcnrhvs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gaaepdere.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gtloowjtm.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gmaywizon.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gzzfbfmqv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/ggfucftzy.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gwlvuvaat.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gmhbtvvjr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/geljizbib.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/glafxhdsj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gcqwlqcbb.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/ghuhkxyat.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gzbpjvoea.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/godgdyibq.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gaohnigev.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gubsdpymw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/graspgisj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gwfnnopny.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gysjxwjks.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gcoknwsel.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/ghlnhbahz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gvxxwydcq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gnxgjqcvi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gtceubxgj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gzmjlumvw.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/geowpjiad.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gegtgqgvo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gqawzjsfu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/giimolyii.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gjzywavbt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gspqulpul.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gxcvwvsdu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/glyinvadg.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gmwedfrtm.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gnmfxrfwg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gwveenzaj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/ggbfrgitd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gjwkejbqz.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gfnrywckp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gdbjeoptg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/grpdoqeej.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/ghiemstgp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gjavqzndn.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gkcxrdnpn.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gtbosycwm.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gmhdmprun.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gmhsmylnl.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gzurxwcyk.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gtphqhaus.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gbcqtvogh.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gjyqtvpao.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gwmwjnkrr.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gzynxrufu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/goraqacpg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gbegcguwi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gcbdnkzeg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/grmoqejpx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gsztlgdsn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gfbhxogov.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/ggpkbtkps.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gdpkbmnjp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gogarjrsd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gvohnmusf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gqavhphpe.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gderhytkw.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gsfwhtuhq.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gukhptqku.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gtvgwfjlg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gvaiaksxv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gbxldcffr.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gktuafyav.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gxficvsoy.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gyuivbyld.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gmerbptkd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gcwxwrpzz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/ghppegjgi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gcnyxireo.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gmuthdbca.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gisldjswu.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gsqftxyul.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/glxwnirsf.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gtsaqzhjw.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gdyywiavh.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/ghczqgeer.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/ghglrpcnl.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/golnoasvu.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gcioplnsk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gxiixzjsh.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gxebhdbgl.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gcmifvdfj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/guxkrwkvy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gvurxkjkk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gqhwypvog.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gqqncdwdh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gxoveqpgs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gbapxmjzk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gwhcbtamd.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gnaqfxgaf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gnpekyrjs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gjjqchwfc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gtlgxxstr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gygddrhqq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gldmfmojb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/guuiawnxr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gbtdbhuge.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/glnbirmyl.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/glrulvhee.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/giartrarp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gltotjxxl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/grxdxbufr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gpeusihjk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gfkzlxtoa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gglidzjyo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/guemtheke.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gaeaucmhr.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gaxlwizep.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gdddqxigb.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gmaskmtba.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gyawxvuvv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gzrddexbd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gjqrdsdbo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gchrbdovm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gbeyquuoh.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gfnleyqml.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gvptqippl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gdlqlpmis.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/guorwromk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gifvlqbhc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gbjizwnzu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gjvrdxypr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/govhvpyhs.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gnwyoqtve.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/ghdenedgh.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gxnfrbyov.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gknyfbsgb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gluqpnihn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/guxmjewfl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gsrdyrmbt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gvfertcvy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gqohnooxd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gqwxzmpei.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gogajogzd.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gemdlswqq.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gbartgbjw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gfcfcubnl.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/ggibgaczn.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gmycndrea.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/glagsfkou.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gnpwhfbrl.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gmxvksrgp.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gzvewahbf.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/grmutsaee.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/grrejmisk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gqqsysnwb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gnbtiytgz.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gcqwfznex.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gwphatorf.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gemvrxtdl.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gmvhpqabx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gwgbfcaba.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gkthrcttl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gwybayduq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gynxgajyf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/glzpdrtsg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gzaavcvfg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gxieqpqnu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gwqwawlmi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/golderclt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gqwmdfcmq.sHtML


<!-- 参考信息 -->